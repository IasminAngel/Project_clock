# Relógio Digital em Python com Tkinter

Este projeto é um relógio digital simples implementado em Python usando a biblioteca Tkinter para criar a interface gráfica. O relógio exibe a hora atual em formato de 12 horas, atualizando a cada segundo.

## Requisitos

- **Python**: Certifique-se de ter Python 3.x instalado. O Tkinter é incluído por padrão com a maioria das instalações do Python.

## Executando o Relógio Digital

1. Salve o código abaixo em um arquivo com a extensão `.py`, por exemplo, `relogio_digital.py`.

2. Execute o script usando o Python:

    ```bash
    python relogio_digital.py
    ```

3. Uma janela será aberta exibindo o relógio digital.

## Código

Aqui está o código completo do relógio digital:

```
from tkinter import *
from time import strftime

# Utilizado para criar funções e em Python

def atualizar_relogio():
    horario_atual = strftime("%H:%M:%S %p")
    rotulo_relogio.config(text= horario_atual)
    rotulo_relogio.after(1000, atualizar_relogio)

janela = Tk()
janela.title("Relógio Digital") 

rotulo_relogio = Label (
        janela,
        font = ("Arial", 40, "bold"),
        background= "pink",
        foreground= "white"
    )

rotulo_relogio.pack(anchor="center")

atualizar_relogio()

janela.mainloop()
```


**Notas:**

1. **Captura de Tela**: Se você deseja incluir uma imagem do relógio digital, adicione-a à pasta `imgs` do seu repositório e substitua o caminho no README pela localização real da imagem.

2. **Links**: Substitua `https://github.com/usuario/repo` pelo URL real do seu repositório no GitHub, e adicione um arquivo de licença (`LICENSE`) se necessário.

3. **Seções de Licença e Contribuições**: Ajuste conforme o tipo de licença e o modelo de contribuição que deseja adotar para o projeto.

