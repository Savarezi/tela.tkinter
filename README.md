# tela.tkinter
**Este projeto demonstra como criar uma janela simples de desktop usando a biblioteca tkint janela . A inclui um rótulo com o texto "Meu Primeiro Código!" e um botão que, quando clicado, imprime uma mensagem no console.** 
import tkinter as tk

# Função para criar e configurar a janela principal
def create_window():
    # Cria a janela principal
    root = tk.Tk()
    
    # Configura o título da janela
    root.title("Minha Janela")
    
    # Define o tamanho da janela
    root.geometry("400x300")  # Largura x Altura
    
    # Cria um rótulo (label) na janela
    label = tk.Label(root, text="Meu Primeiro Código", font=("Arial", 16))
    label.pack(pady=20)  # Adiciona o rótulo à janela com padding vertical
    
    # Cria um botão na janela
    button = tk.Button(root, text="Clique-me", font=("Arial", 14), command=lambda: print("Botão clicado!"))
    button.pack(pady=10)  # Adiciona o botão à janela com padding vertical
    
    # Inicia o loop principal da interface gráfica
    root.mainloop()

# Chama a função para criar a janela
create_window()
