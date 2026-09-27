import random
import customtkinter as ctk

QUOTES = [
    {
        "text": "Talk is cheap. Show me the code.",
        "author": "Linus Torvalds",
    },
    {"text": "Programs must be written for people to read.", "author": "Abelson"},
    {"text": "First, solve the problem. Then, write the code.", "author": "John Johnson"},
]


def show_new_quote():
    item = random.choice(QUOTES)
    quote_label.configure(text=f'"{item["text"]}"')
    author_label.configure(text=f"— {item['author']}")


app = ctk.CTk()
app.geometry("400x200")
app.title("Quote Generator")

quote_label = ctk.CTkLabel(
    app, text="Нажми кнопку!", font=("Helvetica", 14), wraplength=350
)
quote_label.pack(pady=(30, 5))

author_label = ctk.CTkLabel(
    app, text="", font=("Helvetica", 12, "italic"), text_color="gray"
)
author_label.pack(pady=(0, 20))

btn = ctk.CTkButton(app, text="Новая цитата", command=show_new_quote)
btn.pack()

app.mainloop()
