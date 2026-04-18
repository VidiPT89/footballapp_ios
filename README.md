# ⚽ Football App — iOS

An iOS application to follow the **English Premier League**. Browse teams, check the standings table, and save your favourite teams with personal notes and ratings.

Built as a course project at CESAE Digital, using SwiftUI with MVVM architecture.

---

## ✨ Features

- 📋 List of all Premier League teams
- 🏟️ Team details — badge, stadium, founding year, club colours, and official website
- 📊 Standings table with colour-coded zones (Champions League, Europa League, Relegation)
- ⭐ Favourites management — add, remove, and reorder
- 📝 Personal notes and star ratings (1–5) per favourite team
- 💾 Local persistence of favourites using SwiftData

---

## 🛠️ Technical Foundation

| Component | Technology |
|---|---|
| Language | Swift 5.9 |
| UI Framework | SwiftUI |
| Architecture | MVVM with `@Observable` |
| Local Persistence | SwiftData |
| API | football-data.org v4 |
| Async Images | `AsyncImage` |
| Navigation | `NavigationStack` + `TabView` |

---

## 📱 Available Screens

| Screen | Description |
|---|---|
| Teams | Full team list with favourite toggle |
| Team Detail | Complete team info + link to official website |
| Standings | Table with positions and colour-coded zones |
| Favourites | Saved teams sorted by date added |
| Favourite Detail | Team info alongside personal note and rating |
| Edit Favourite | Form to update personal rating and notes |

---

## ⚙️ Requirements

- Xcode 15 or later
- iOS 17 or later
- Valid API key from [football-data.org](https://www.football-data.org/)

---

## 🗒️ Developer Notes

- The API token is hardcoded in `APIHandler.swift` — in a production environment it should be managed securely (e.g. `.xcconfig` or Keychain)
- The app is limited to the Premier League (code `PL`); the API supports other competitions
- Variable and view names are written in Portuguese, following the course project convention
- First iOS project using SwiftUI and SwiftData

---

## 🎓 Academic Context

Project developed as part of a programming course at **CESAE Digital**, as an introduction to native iOS development with SwiftUI.
