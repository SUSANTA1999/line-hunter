# Line Hunter - Zoom Meeting Subscription Service

A single-page web application that provides subscription-based Zoom meeting access with unified user and admin panels.

## Features

### 🔐 Unified Authentication
- Single login box for both users and admins
- Role-based access control
- Admin can create user accounts (users cannot self-register)

### 👤 User Panel
- Subscription status display (Active, Expired, Inactive)
- Plan information (Weekly, Monthly)
- Start and expiry dates
- Real-time countdown timer to expiry
- "Join Line" button with Zoom icon
- User-specific Zoom meeting links
- Auto-hide join button when subscription expires

### 🛡️ Admin Panel
- Create new user accounts
- Assign user-specific Zoom links
- Manage subscription plans and status
- View all users in a table format
- Edit and delete user accounts
- Set subscription expiry dates

### 🎨 Modern UI
- Responsive design with Tailwind CSS
- Beautiful gradient backgrounds
- Smooth animations and transitions
- Font Awesome icons
- Mobile-friendly interface

## Default Login Credentials

### Admin
- User ID: `admin001`
- Password: `admin123`

### Sample User
- User ID: `john001`
- Password: `password123`

## How to Use

1. **Open the Application**: Open `index.html` in your web browser
2. **Admin Login**: Click "Admin Access" and use admin credentials
3. **Create Users**: In admin panel, create new user accounts with their Zoom links
4. **User Login**: Users can login with their credentials
5. **Join Meetings**: Active users can click "Join Line" to open their Zoom meeting

## Data Storage

- Currently uses browser's localStorage for data persistence
- In production, this should be replaced with a backend database
- All user data, subscriptions, and Zoom links are stored locally

## Customization

### Adding New Users
Only admins can create new user accounts. Users cannot self-register for security reasons.

### Subscription Plans
- Weekly: 7 days from start date
- Monthly: 30 days from start date

### Zoom Integration
Each user gets a unique Zoom meeting link assigned by the admin. The "Join Line" button opens the user's specific Zoom meeting.

## Technical Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Tailwind CSS
- **Icons**: Font Awesome
- **Storage**: LocalStorage (for demo purposes)

## Future Enhancements

- Backend database integration
- Payment gateway integration
- Email notifications for expiry
- Bulk user management
- Advanced analytics dashboard
- Multi-language support

## License

This project is open source and available under the MIT License.
