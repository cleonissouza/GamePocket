# 🎮 GamePocket

GamePocket is an Android application for browsing and managing favorite games, utilizing the RAWG.io API. The project features a modular architecture, including integration with the local Room database and communication via Retrofit.

## 📱Features
	•	Home screen displaying a list of popular games.
	•	Search for games by name.
	•	Detailed view of each game, including description, image, and release date.
	•	Recommended games list within the details screen.
	•	Saving favorite games to the local database (Room).
	•	Viewing the list of favorite games.
	•	Screen navigation using the Navigation Component.

---

## 🛠️ Technologies and Libraries Used
	•	Language: Kotlin
	•	Architecture: MVVM (Model - View - ViewModel)
	•	Networking: Retrofit + Gson
	•	Database: Room Database
	•	Coroutines & Flow: For asynchronous operations and reactivity
	•	Navigation Component: For navigation management
	•	ViewBinding: For view handling
	•	Glide: For image loading
	•	Material Design 3: For modern UI components

---

## 🌐 API Used  
	•	RAWG.io – Game data platform.  

Implemented endpoints:  
	•	GET /games – Game list  
	•	GET /games/{id} – Details of a specific game  
	•	GET /games/{id}/suggested – List of recommended games  


## :camera_flash: Screenshots
<img width="200" src="https://github.com/user-attachments/assets/74a74b71-1fde-4ab3-a32f-8c214bb2b077" />
<img width="200" src="https://github.com/user-attachments/assets/03103576-764b-4332-833c-2209c279203c" />
<img width="200" src="https://github.com/user-attachments/assets/b677be4c-8323-4246-9dd9-d77da64166e6" />
<img width="200" src="https://github.com/user-attachments/assets/fd16600d-44cf-415d-b12d-cf5be79f4340" />
<img width="200" src="https://github.com/user-attachments/assets/4d464969-f5e7-4107-b349-a6104bbef90a" />


  
⸻  

✅ What’s Been Done

API Integration  
	•	Retrofit configured and tested  
	•	Game listing, details, and recommended endpoints integrated  
	•	Support for search and sorting parameters  
	•	Detailed logging in Logcat for debugging  

Local Database (Room)  
	•	Local database created  
	•	Favorite games entity set up   
	•	DAO with insert, delete, and query methods  
	•	Repository integrated with Room  

Fragments and ViewModels  
	•	HomeFragment: Displays popular games  
	•	SearchFragment: Search for games via API  
	•	DetailFragment: Full game details and recommended games  
	•	FavoriteFragment: List of locally stored favorite games  

Adapters and UI  
	•	RecyclerView with adapter configured  
	•	ViewBinding used for view handling  
	•	Glide for image loading  
	•	Favorite button using IconToggleButton (with future Compose migration)  

Navigation  
	•	Navigation Component configured with nav_graph.xml  
	•	Complete flow: Home ➜ Detail ➜ Favorite ➜ Favorites List  

⸻

🚀 Next Steps (For the Team)  
	•	Improve UI/UX:  
	•	Fully apply Material Design 3  
	•	Create responsive layouts for tablets  
	•	Implement animations and transitions  
	•	Error Handling:  
	•	Create error screens (e.g., no internet, 404 error)  
	•	Add loading indicators (Shimmer or ProgressBar)  
	•	Pagination:  
	•	Implement infinite scroll in Home and Search screens  
	•	Favorites:  
	•	Add visual feedback (Snackbar or Toast) when favoriting/unfavoriting  
	•	Testing:  
	•	Create unit tests for ViewModels and Repository  
	•	Create instrumentation tests for full flow  
	•	Code Refinement:  
	•	Implement a UiState layer to handle states (Loading, Success, Error)  
	•	Review and clean up excessive logging  
 
⸻  

⚠️ Important Notes  
	•	The API key (Constants.API_KEY) should be protected. It’s recommended to migrate to a secure solution in the future (e.g., Remote Config or Keystore).  
	•	The project is fully functional and ready for continued UI development.  

⸻

📚 References  
	•	RAWG.io Documentation  
	•	MVVM Architecture with Flow  
	•	Material Design 3 Guide  

⸻

🧑‍💻 Developed by  

Team 3 HackSprint DevSpace, initiated by [Robson Santos, Francisco Souza, Elieudo Silva, Geovâneo dos Santos Souza].  

⸻  

📦 Environment Requirements  
	•	Android Studio Flamingo or newer  
	•	Kotlin 1.8+  
	•	MinSDK 24  
	•	TargetSDK 34  
	•	Emulator or physical device with internet access  

⸻

🏁 How to Run  

```bash
git clone <repository>
cd GamePocket
./gradlew assembleDebug
