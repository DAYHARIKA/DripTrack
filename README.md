# DripTrack
DripTrack - Wardrobe Manager

Ever feel like you have nothing to wear, even though your wardrobe is packed? DripTrack is here to change that. It helps you keep track of what clothes you already have and how often you wear them—all from your phone. No more digging through piles or buying clothes you don’t need. Just scroll through your wardrobe, mix and match outfits, and you’ll always know what you’ve got. Plus, by reducing unnecessary purchases, we’re all about sustainability and keeping your wardrobe organized.

Key Features:
1. User Login (Authentication) Status: Completed
Problem: I need to make sure users can log in and their data is safe.
Solution: Implement a secure login system with JWT tokens to manage user sessions. This way, each user’s wardrobe data is separate.
Auth Screenshot
<img width="1919" height="1079" alt="Auth" src="https://github.com/user-attachments/assets/bff57db7-d1fb-406d-8d7a-2c9b47a6ac43" />

2. Stats - Track Your Wardrobe Usage Status: Complete
Problem: Users need insights into their wardrobe usage, such as how many times they've worn certain items.
Solution: Add a Stats page that displays key wardrobe statistics like total items, most worn items, and usage frequency for each item.
Stats Screenshot
<img width="1892" height="1079" alt="Stats" src="https://github.com/user-attachments/assets/27d75eee-464d-4546-8636-a7d392672735" />

4. Wardrobe Management (Adding Items) Status: Completed
Problem: Users need to upload their clothes and categorize them.
Solution: Provide a form where users can upload photos and manually assign categories like “shirts,” “pants,” and more.
   
<img width="1918" height="1079" alt="Upload" src="https://github.com/user-attachments/assets/d7d71d3b-e7b6-4f1e-aca2-506110ecc505" />
<img width="1912" height="1079" alt="closet" src="https://github.com/user-attachments/assets/3e0f06ec-b886-440b-97c5-474437b80736" />

5. Usage Tracking Status: Completed
Problem: How do users keep track of how often they wear an item?
Solution: Create a button that allows users to mark when they wear an item, which increments a counter for that item’s usage.
<img width="1912" height="1079" alt="closet" src="https://github.com/user-attachments/assets/3e0f06ec-b886-440b-97c5-474437b80736" />

7. Sorting by Usage Status: Completed
Problem: How can users see which items they wear the most or least?
Solution: Add sorting functionality that allows users to sort their wardrobe items by usage (ascending/descending).
Sort Screenshot
<img width="1912" height="1079" alt="closet" src="https://github.com/user-attachments/assets/3e0f06ec-b886-440b-97c5-474437b80736" />

8. Fashion AI Chatbot Status: Completed
Problem: Users want personalized fashion advice and help with outfit choices.
Solution: Add an AI-powered chatbot to answer fashion-related questions. The chatbot will respond with helpful tips, such as suggesting outfits, answering questions about items in the wardrobe, and providing general fashion advice based on trends and user preferences.
Chat Screenshot
<img width="1912" height="1079" alt="closet" src="https://github.com/user-attachments/assets/3e0f06ec-b886-440b-97c5-474437b80736" />

9. Wishlist - Save for Later Status: Completed
Problem: Users often find items they like but aren't ready to buy yet, leading to lost finds or impulse purchases.
Solution: A dedicated Wishlist section where users can save items they want to buy. Includes a "Move to Closet" feature to easily transfer items once purchased.
Wishlist Screenshot
<img width="1912" height="1079" alt="closet" src="https://github.com/user-attachments/assets/3e0f06ec-b886-440b-97c5-474437b80736" />

11. Outfit Creator (Mix & Match) Status: Completed
Problem: Having clothes is one thing, but knowing how to combine them into outfits is another.
Solution: An interactive "Mix & Match" interface. Users can select multiple items from their digital closet to create, name, and save full outfits (e.g., "Date Night", "Office Wear").
Outfit Creator Screenshot
<img width="1912" height="1079" alt="closet" src="https://github.com/user-attachments/assets/3e0f06ec-b886-440b-97c5-474437b80736" />

Folder Architecture
DripTrack/
├── backend/
│   ├── config/             # DB and Cloudinary configuration
│   ├── middleware/         # Auth verification
│   ├── models/             # Mongoose models (User, ClosetItem, WishlistItem, Outfit)
│   ├── routes/             # API routes (auth, closet, wishlist, outfit)
│   ├── .env                # Environment variables
│   └── server.js           # Entry point
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/         # Images, fonts, icons
│   │   ├── components/
│   │   │   ├── Auth/       # Login/Signup forms
│   │   │   ├── basics/     # Layout components (Navbar, Footer)
│   │   │   ├── ClosetForm.jsx
│   │   │   ├── ClosetList.jsx
│   │   │   ├── Modal.jsx   # AI Chatbot Modal
│   │   │   ├── OutfitCreator.jsx
│   │   │   ├── Stats.jsx
│   │   │   ├── Wishlist.jsx
│   │   │   └── ...
│   │   ├── lib/            # Gemini AI configuration
│   │   ├── App.jsx         # Routing
│   │   └── main.jsx
│   ├── .env                # Frontend environment variables
│   ├── index.html
│   ├── tailwind.config.js
│   └── vite.config.js
└── README.md

Tech Stack
Frontend:
React.js - Vite - Tailwind CSS - Backend:
Node.js - Express.js - MongoDB - Google Cloud Platform
Challenges I Faced
Managing Image Uploads: Figuring out how to handle image uploads securely and efficiently.
Real-Time Updates: Keeping the wardrobe data up-to-date with real-time usage tracking.
Mobile Responsiveness: Ensuring the app looks good on all devices (mobile-first design with Tailwind).
End Goal
To have a simple but effective wardrobe management app that helps people keep their clothes organized and track what they wear the most. Eventually, I might even add AI to recommend outfits based on what you wear most often.

Stay tuned! 🚀
