# DZCORE Control Center

Separate moderation dashboard for DZCORE.

## Features

- Secret-protected admin login
- User, post, comment, report and ban metrics
- Search users by username, display name or email
- Temporary/permanent ban and unban
- Admin warning notifications
- Safe temporary password reset (original passwords are never readable)
- Report queue with resolve action

The dashboard calls the DZCORE Cloudflare API at `https://dzcore.top` by default. Set `VITE_DZCORE_API` for another API endpoint.

## Security

The secret is checked server-side. Do not place it in this repository or frontend source. User passwords are stored as salted PBKDF2 hashes and are never returned by the API.
