# 🌲 Timber!!! - C++ Game

![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![SFML](https://img.shields.io/badge/SFML-8CC445?style=for-the-badge&logo=sfml&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)

Um clone do clássico arcade **Timberman**, desenvolvido em **C++** utilizando a biblioteca **SFML**. Este projeto foi um marco inicial nos meus estudos de desenvolvimento de jogos, focando em conceitos fundamentais de lógica, renderização e gerenciamento de recursos.

## 🕹️ O Jogo

O objetivo é simples: você é um lenhador que precisa cortar a árvore o mais rápido possível enquanto desvia dos galhos que descem. 

- **Desafio:** A barra de tempo diminui constantemente. Quanto mais você corta, mais tempo ganha, mas a velocidade do jogo também aumenta!
- **Ambiente:** Inclui elementos animados como nuvens, abelhas e efeitos de movimentação.

## 🚀 Tecnologias Utilizadas

* **Linguagem:** C++
* **Biblioteca Gráfica:** SFML (Simple and Fast Multimedia Library)
* **Gerenciamento de Tempo:** Sistema de `sf::Clock` para controle do Game Loop.

## 🛠️ Como Compilar e Rodar

Este projeto foi desenvolvido utilizando a versão **SFML 2.x**. Devido a mudanças significativas na API da versão 3.0 (como a remoção de construtores padrão e alterações no sistema de eventos), é necessário utilizar a versão **2.6.2** para garantir a compatibilidade.

### Passo 1: Baixar a SFML 2.6.2
1. Faça o download da versão **Linux 64-bit** no site oficial: [SFML 2.6.2 Download](https://www.sfml-dev.org/download/sfml/2.6.2/).
2. Extraia o conteúdo na raiz do projeto para que a pasta fique como `./SFML-2.6.2`.

### Passo 2: Compilar e Rodar (Linux)
Como estamos usando uma versão local da biblioteca (fora dos diretórios padrão do sistema), precisamos apontar os caminhos manualmente para o compilador e para o carregador de bibliotecas do Linux:

```bash
# 1. Clonar o repositório
git clone https://github.com/guicpaiva/Timber.git
cd Timber

# 2. Compilar o objeto apontando para os headers locais
g++ -c main.cpp -I ./SFML-2.6.2/include

# 3. Linkar os binários apontando para as bibliotecas locais
g++ main.o -o timber-game -L ./SFML-2.6.2/lib -lsfml-graphics -lsfml-window -lsfml-system

# 4. Executar definindo o caminho das bibliotecas compartilhadas
LD_LIBRARY_PATH=./SFML-2.6.2/lib ./timber-game
Nota: Se você estiver em uma distro Arch/CachyOS e encontrar erros de "no matching function", certifique-se de que não há uma versão global da SFML 3.x instalada no sistema que possa estar conflitando com os headers locais.
```

## 📚 Créditos e Referências

Este projeto foi desenvolvido como um exercício prático seguindo o guia do livro:

Livro: Beginning C++ Game Programming
Autor: John Horton
Editora: Packt Publishing
