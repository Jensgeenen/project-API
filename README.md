# To-Do List API

Dit project is een eenvoudige To-Do List API waarmee gebruikers taken kunnen beheren. Gebruikers kunnen taken aanmaken, bijwerken, verwijderen, en ophalen. Taken kunnen worden gekoppeld aan projecten en gebruikers. De API is gebouwd met Flask en gebruikt SQLite als database.

## Entiteiten
- **User**: Gebruikers die taken en projecten kunnen beheren.
- **Task**: Taken die door gebruikers kunnen worden aangemaakt en gekoppeld aan projecten.
- **Project**: Projecten waaraan taken gekoppeld kunnen worden.

## API Endpoints

### GET /tasks
Haalt alle taken op.

### GET /tasks/<int:id>
Haalt een specifieke taak op basis van ID.

### POST /tasks
Maakt een nieuwe taak aan. Vereiste velden:
- `title`: De titel van de taak.
- `description`: Een optionele beschrijving van de taak.
- `due_date`: De vervaldatum van de taak (YYYY-MM-DD).
- `user_id`: De ID van de gebruiker die de taak aanmaakt.
- `project_id`: De ID van het project waaraan de taak is gekoppeld.

### PUT /tasks/<int:id>
Werkt een bestaande taak bij.

### DELETE /tasks/<int:id>
Verwijdert een specifieke taak.
