Encrypted Journal
A secure, password-protected personal journal application built with vanilla HTML, CSS, and JavaScript. Keep your thoughts and reflections private with client-side encryption.
Features
🔐 Security & Privacy
•	Client-side encryption: All data is encrypted using a simple XOR cipher before being stored locally
•	Password protection: Master password required to access your journal
•	Local storage: All data stays on your device - no server required
✍️ Journaling Features
•	Rich writing interface: Clean, distraction-free writing environment
•	Mood tracking: Select from 8 different moods for each entry
•	Writing prompts: Built-in inspiration prompts plus custom prompt management
•	Entry management: Edit, delete, and restore journal entries
📚 Organization & Discovery
•	Monthly filtering: Browse entries by specific months and years
•	Full-text search: Search through all your entries
•	Random entry: Discover forgotten memories with random entry selection
•	Trash system: Soft delete with restore functionality
🎨 User Experience
•	Responsive design: Works on desktop, tablet, and mobile devices
•	Modern UI: Clean, gradient-based design with smooth animations
•	Intuitive navigation: Tab-based interface for easy access to all features
•	Visual feedback: Success/error messages and loading states
Getting Started
Prerequisites
•	A modern web browser (Chrome, Firefox, Safari, Edge)
•	No additional software or server setup required
Installation
1.	Download the index.html file (or the complete project)
2.	Open the file in your web browser
3.	That's it! The application runs entirely in your browser
First Time Setup
1.	Open the application in your browser
2.	Enter any password of your choice (this will be your master password)
3.	Click "Unlock Journal" to create your encrypted journal
4.	Remember your password - you'll need it to access your entries
Usage
Writing Entries
1.	Navigate to the Write tab
2.	Use the inspiration prompts for ideas or start writing directly
3.	Select your current mood from the mood selector
4.	Click "Save Entry" to encrypt and store your reflection
Reading Entries
1.	Go to the Read tab
2.	Use month filters to browse entries by time period
3.	Edit or delete entries using the action buttons
4.	Entries are displayed with date, mood, and full text
Searching
1.	Visit the Search tab
2.	Type keywords to find specific entries
3.	Search works across entry text and mood tags
Random Discovery
1.	Click the Random tab
2.	Use "Show Random Entry" to rediscover past reflections
3.	Perfect for nostalgic moments or reflection
Managing Prompts
1.	Access the Prompts tab
2.	Add custom writing prompts to inspire future entries
3.	Click any prompt to start writing with that inspiration
Trash Management
1.	Deleted entries are moved to the Trash tab
2.	Restore accidentally deleted entries
3.	Permanently delete entries when ready
Security Notes
Encryption Details
•	Uses a simple XOR cipher for client-side encryption
•	Password is used as the encryption key
•	Important: This is basic encryption suitable for personal privacy, not military-grade security
Data Storage
•	All data is stored in your browser's localStorage
•	Data persists between browser sessions
•	Clearing browser data will remove all entries
•	Backup recommendation: Export your data periodically
Password Security
•	Choose a strong, memorable password
•	Lost password = lost data - there's no recovery method
•	Consider using a password manager
•	Password is never transmitted or stored anywhere
Browser Compatibility
Supported Browsers
•	Chrome/Chromium 60+
•	Firefox 55+
•	Safari 11+
•	Edge 79+
Required Features
•	localStorage support
•	ES6 JavaScript features
•	CSS3 animations and transforms
•	Font Awesome icons (loaded from CDN)
Technical Details
File Structure
encrypted-journal/
├── index.html          # Complete application (HTML, CSS, JS)
└── README.md          # This file
Dependencies
•	Font Awesome 6.4.0 (loaded from CDN)
•	No other external dependencies
Key Functions
•	simpleEncrypt() / simpleDecrypt(): Handle data encryption/decryption
•	saveData() / loadData(): Manage localStorage operations
•	handleLogin(): Authentication and data decryption
•	handleSaveEntry(): Entry creation and editing
•	Tab management and UI updates
Customization
Styling
•	Modify CSS variables in the <style> section
•	Gradient backgrounds can be changed in the body selector
•	Color scheme is defined at the top of the CSS
Prompts
•	Default prompts are in the inspirationList initialization
•	Custom prompts can be added through the UI
•	Modify the default prompts in the HTML section
Moods
•	Mood options are defined in the HTML mood selector
•	Add new moods by modifying the .mood-option elements
•	Update the getMoodEmoji() function for new mood emojis
Troubleshooting
Common Issues
"Incorrect password" error
•	Ensure you're using the exact same password as when you created the journal
•	Password is case-sensitive
•	Clear browser cache and try again if issues persist
Entries not loading
•	Check browser console for JavaScript errors
•	Ensure localStorage is enabled in your browser
•	Try refreshing the page
Styling issues
•	Ensure Font Awesome CDN is accessible
•	Check if browser supports CSS Grid and Flexbox
•	Try a different browser to isolate the issue
Data loss prevention
•	Regularly backup your entries by copying the encrypted data from localStorage
•	Don't clear browser data without backing up first
•	Consider using the same browser consistently
Privacy & Data Handling
What's Stored
•	Encrypted journal entries
•	Encrypted mood data
•	Encrypted custom prompts
•	Encrypted trash entries
•	All data is stored locally in your browser
What's NOT Stored
•	Your master password (only used for encryption/decryption)
•	Any data on external servers
•	Personal information beyond what you write
Data Portability
•	Data is stored in localStorage as encrypted JSON
•	Manual export/import would require additional development
•	Consider implementing backup features for important journals
Contributing
This is a single-file application perfect for personal use and learning. Potential improvements:
Suggested Enhancements
•	Export/import functionality
•	Stronger encryption algorithms
•	Rich text editing capabilities
•	Image attachment support
•	Cloud sync options
•	Multiple journal support
•	Advanced search filters
•	Data visualization (mood trends, writing frequency)
Development Setup
1.	Clone or download the file
2.	Open in any text editor
3.	Make modifications to HTML, CSS, or JavaScript
4.	Test in browser
5.	No build process required
License
This project is provided as-is for personal use. Feel free to modify and distribute according to your needs.
Support
For issues or questions:
1.	Check the troubleshooting section above
2.	Inspect browser console for error messages
3.	Test in different browsers to isolate issues
4.	Consider the technical limitations of client-side encryption
________________________________________
Remember: This journal is only as secure as your password and browser security. For highly sensitive information, consider using dedicated encrypted note-taking applications with stronger security features.
