def build_note(note_text, note_name):
    with open(f"{note_name}.txt", "w", encoding="utf-8") as file:
        file.write(note_text)
    print(f"Заметка {note_name} создана.")
   def create_note():
    note_name = input("Введите название заметки: ")
    note_text = input("Введите текст заметки: ")
    build_note(note_text, note_name)
    notes = [note for note in os.listdir() if note.endswith(".txt")]
    def build_note(note_text, note_name):
    try:
        with open(f"{note_name}.txt", "w") as file:
            file.write(note_text)
        print(f"Заметка {note_name} создана.")
