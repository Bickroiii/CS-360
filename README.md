# CS-360

Application Description and Icon 
The mobile application developed for this project is an inventory tracking app designed to 
help users manage and monitor stock levels in a simple and organized way. The app allows 
users to create accounts, log in securely, and store inventory data in a persistent database 
so information is not lost when the app is closed. Users can add new inventory items, 
update existing quantities, delete items that are no longer needed, and view all stored 
items in a grid layout that makes information easy to read and navigate. In addition, the 
application includes an optional SMS alert feature that notifies users when inventory levels 
fall below a defined threshold. This feature helps users avoid shortages and encourages 
proactive inventory management. 
If the application were published in an app store, the description would emphasize its 
simplicity, reliability, and usefulness for everyday users and small business owners. The 
description would highlight account based access, persistent database storage, easy grid 
visualization, and optional SMS notifications for low inventory. The application would be 
positioned as a lightweight and accessible solution for inventory management without 
requiring complex enterprise software. 
The app icon should visually represent organization and stock tracking. A suitable design 
would be a storage box paired with a checklist overlay to communicate the idea of 
managing inventory. This icon concept is simple, recognizable, and consistent with Android 
design guidelines that emphasize clarity and scalability across different device sizes. 
Android Version Compatibility 
The application was developed with a minimum SDK version that supports Android 8.0 and 
higher. This decision ensures that the app can run on a wide range of devices while still 
supporting modern development features and security requirements. Supporting older 
versions of Android improves accessibility for users who may not have the latest devices, 
while still maintaining compatibility with current Android platform standards. 
The application was also tested using recent Android emulator images to confirm that it 
functions properly on newer versions of the operating system. Supporting current Android 
versions is important because each release introduces updates to security, permissions, 
and system behavior that can impact application performance. By targeting both a 
minimum supported version and the latest Android version, the application balances 
accessibility with long term stability. 
Future updates may incorporate additional platform features such as improved notification 
management and enhanced user privacy controls. Planning for forward compatibility 
ensures the application can evolve alongside Android platform advancements. 
Application Permissions 
The application requests only permissions that are necessary for its intended functionality. 
This approach reflects responsible development practices and helps maintain user trust by 
avoiding unnecessary access to device features. 
The primary permission required is SMS messaging capability. This permission supports 
the low inventory alert feature that sends a text message when item quantities fall below a 
specified level. The permission is requested at runtime so users can decide whether they 
want to enable SMS notifications. If the user denies permission, the application continues 
to function normally, allowing inventory tracking and database operations without 
interruption. 
No additional permissions are required because the application does not use location 
services, microphone input, camera access, or internet connectivity for its core 
functionality. Limiting permissions improves security, reduces privacy concerns, and aligns 
with best practices for mobile application deployment. 
Monetization Strategy 
The monetization strategy for the inventory application follows a freemium approach that 
prioritizes accessibility while allowing opportunities for future revenue generation. The 
base version of the application is free and includes full inventory management 
functionality, including account creation, database storage, grid visualization, and manual 
inventory tracking. 
Future premium features may include advanced analytics, reporting capabilities, cloud 
backup support, and expanded notification customization. These features could be offered 
through a one time purchase or optional subscription depending on user demand and 
future development goals. 
Another possible monetization approach is the inclusion of minimal and non intrusive 
advertisements within the application interface. Ads would be implemented in a way that 
does not interfere with the user experience or core functionality. This strategy allows users 
to continue using the application for free while generating supplemental revenue. 
The freemium model supports broader adoption by lowering barriers to entry while 
providing flexibility for sustainable growth. This approach also allows user feedback to 
guide future enhancements and feature expansion. 
Conclusion 
The inventory tracking application provides a practical and user friendly solution for 
managing stock data in personal and small business contexts. The launch plan focuses on 
clear application positioning, thoughtful icon design, broad Android compatibility, 
responsible permission usage, and a flexible monetization strategy. Together, these 
components establish a strong foundation for preparing the application for distribution and 
future development. 
By emphasizing usability, privacy awareness, and scalability, the application aligns with 
modern mobile development expectations. This launch plan demonstrates readiness for 
deployment while supporting opportunities for continued improvement and feature 
expansion as the application evolves.


Project Reflection
Application Summary and User Needs

The goal of this application was to develop a fully functional inventory tracking system that allows users to securely log in, manage inventory items, and receive optional low stock notifications. The application was designed to address the needs of individuals or small business owners who require a simple and reliable way to track inventory levels without complex enterprise software. By providing persistent database storage through SQLite, users are able to create, read, update, and delete inventory items while ensuring their data is not lost when the app closes. The optional SMS alert feature further supports proactive inventory management by notifying users when quantities fall below a defined threshold.

Screens, Features, and User Centered Design

The application required multiple screens and features to support user needs effectively. The login screen was necessary to provide secure account access and allow new users to create credentials. The inventory screen was designed with a grid layout to make item information easy to view and navigate. Features such as add, update, and delete functionality were essential to allow full CRUD operations within the database.

The user interface was intentionally kept clean and minimal to reduce cognitive load. Buttons were clearly labeled, input fields were intuitive, and layout spacing was consistent to improve readability. The grid layout helped present inventory data in a structured format that feels organized and easy to scan. The SMS permission request was handled at runtime to give users control over their privacy. These design decisions ensured the application remained simple, functional, and user focused.

Coding Approach and Development Strategy

The development process began by structuring the application into logical components, including activities, a database helper class, and a RecyclerView adapter. Breaking the application into smaller components made the project more manageable and allowed each piece to be tested independently. I followed a structured approach by first implementing login functionality, then database creation, followed by CRUD operations, and finally SMS permission handling.

Inline comments and clear naming conventions were used to maintain readability and organization. Debugging tools within Android Studio, such as breakpoints and Logcat, were used to identify issues and verify database behavior. This structured and modular approach can be applied to future projects by ensuring that functionality is built incrementally and tested consistently throughout development.

Testing and Validation

Testing was performed using the Android Emulator. I tested account creation, login validation, database persistence, CRUD operations, and SMS permission responses. Both scenarios for SMS permissions were tested to ensure the app continued functioning even when permission was denied. Breakpoints were set in key methods such as login validation and database updates to confirm correct execution flow.

This testing process was important because it revealed potential issues early, such as layout mismatches and permission handling errors. Continuous testing ensured that functionality remained stable as new features were added. It also reinforced the importance of validating user input and handling edge cases to prevent crashes.

Innovation and Problem Solving

One challenge during development was integrating runtime SMS permissions while ensuring the rest of the application remained functional if permission was denied. Implementing conditional logic to allow the app to continue operating required careful planning. Additionally, organizing the SQLite database structure in a way that supported both user authentication and inventory management required thoughtful design.

Overcoming these challenges involved reviewing Android documentation, refactoring code for clarity, and restructuring components to maintain separation of concerns. This experience strengthened my ability to troubleshoot and adapt when facing technical obstacles.

Areas of Success

A particularly strong component of the application was the integration of SQLite database functionality with the RecyclerView grid interface. Successfully implementing full CRUD operations while maintaining persistent storage demonstrated an understanding of database management within a mobile application environment. The login system and runtime SMS permission handling also showcased knowledge of Android security practices and user privacy considerations.
