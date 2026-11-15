🐾 FloquinhoApp
> A modern Android application built with Jetpack Compose and Kotlin (optimized for mobile development environments like AndroidIDE), featuring the daily life and charisma of Floquinho (a caramel and cream Pomeranian). The app includes dynamic theming, GitHub-based developer friend management, and a robust internationalization system powered by custom property files called .flang.
> 
📄 The .flang Format (Floquinho Language)
.flang is the proprietary configuration and translation file format of FloquinhoApp. Inspired by .properties files, it combines global metadata, state counters (such as pet affection), and a complete dictionary of keys and values.
Standard Structure of a .flang File
# Control and Identification Metadata
createNewLang=false
langModification=en
langName=English
affectionData=42

# UI Translation Dictionary (Key = Translated Value)
tab_inicio=Home
tab_comunidade=Community
tab_amizades=Friends
tab_config=Config.
hero_title=Hi, I'm Floquinho!
hero_bio=Cream & caramel Pomeranian, expert at smiling for photos and asking for belly rubs.
card_breed_title=Coat & Size
card_breed_desc=Fluffy cloud with perky ears and the happiest smile in town.
card_mood_title=Current Mood
card_mood_desc=100% joyful, ready to play in the living room or get treats.
card_snack_title=Favorite Treat
card_snack_desc=Crunchy chicken biscuits and tiny apple slices.
friends_status=Developer pup friends
comm_title=Community Translations
comm_editing=Editing
comm_new_lang_btn=Create New Language
comm_confirm_btn=Confirm and Apply Language
comm_success=Translation saved successfully!
comm_dialog_title=Create New Language
comm_dialog_label=Name (e.g., Español)
comm_dialog_create=Create
comm_dialog_cancel=Cancel
friends_header=Add Pup Friend via GitHub
friends_name_label=Developer Name (Optional)
friends_link_label=GitHub link or username
friends_add_btn=Identify and Add Pup Friend
config_header=Settings & Storage
config_snack_alert=Treat Alerts
config_snack_desc=Remember to give snacks to Floquinho
config_storage_title=Storage Manager (Translations)
config_export_btn=Export
config_import_btn=Import
config_active_lang=Active App Language
affection_info=Affection

🔑 Complete Dictionary of Keys (TRANSLATION_KEYS)
The app ecosystem strictly recognizes the following keys to dynamically render texts in any imported language:
| Key (keyName) | Description / UI Location |
|---|---|
| tab_inicio | Home tab label on the bottom navigation bar. |
| tab_comunidade | Community / Translations tab label. |
| tab_amizades | Developer Pup Friends tab label. |
| tab_config | Settings and Storage tab label. |
| hero_title | Main greeting header on the home screen. |
| hero_bio | Detailed bio profile description of Floquinho. |
| card_breed_title | Title for the Coat & Size card. |
| card_breed_desc | Detailed description of the breed and characteristics. |
| card_mood_title | Title for the Current Mood card. |
| card_mood_desc | Description of the pet's current state of mind. |
| card_snack_title | Title for the Favorite Treat card. |
| card_snack_desc | Description of preferred snacks. |
| friends_status | Header for the developer pup friends list. |
| comm_title | Main header for the community translations screen. |
| comm_editing | Label indicating the active language being edited. |
| comm_new_lang_btn | Button text to create a new language from scratch. |
| comm_confirm_btn | Button to confirm and apply translation changes. |
| comm_success | Success message displayed when saving translation packages. |
| comm_dialog_title | Title for the new language creation dialog. |
| comm_dialog_label | Input field label for the new language name. |
| comm_dialog_create | Creation confirmation button inside the dialog. |
| comm_dialog_cancel | Cancellation button inside the dialog. |
| friends_header | Header for the section adding new pup friends via GitHub. |
| friends_name_label | Optional field for the developer friend's name. |
| friends_link_label | Field to enter the GitHub profile link or username. |
| friends_add_btn | Button to fetch avatar and add the pup friend to the list. |
| config_header | Main title for the Settings tab. |
| config_snack_alert | Label for the treat alert switch. |
| config_snack_desc | Description for the snack reminder feature. |
| config_storage_title | Section title for the storage manager and .flang files. |
| config_export_btn | Native button to export the current .flang file. |
| config_import_btn | Native button to import and load .flang files. |
| config_active_lang | Radio selector to toggle the active app language. |
| affection_info | Dynamic text for the pet affection counter. |
🚀 Key Features
 * Native .flang Storage: Import and export translation files using native Android document selectors (ACTION_OPEN_DOCUMENT and ACTION_CREATE_DOCUMENT).
 * GitHub Integration: Dynamically add developer friends by providing just their link or username, automatically generating avatars via Coil and allowing entries to be favorited or deleted.
 * Affection Mode & Persistent Counter: Interactive pet affection counter synchronized and saved within SharedPreferences and the .flang schema.
 * Immersive Design: Built entirely in Jetpack Compose with Material 3 support, custom solid black system bars, and smooth scrolling.
