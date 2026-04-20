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

Certifique-se de ter a biblioteca **SFML** instalada em seu sistema.

### No Linux (Arch/CachyOS)
```bash
# Instalação da SFML
sudo pacman -S sfml

# Clonar o repositório
git clone [https://github.com/guicpaiva/Timber.git](https://github.com/guicpaiva/Timber.git)
cd Timber

# Compilação
g++ -c main.cpp
g++ main.o -o timber-game -lsfml-graphics -lsfml-window -lsfml-system

# Executar
./timber-game
```

## 📚 Créditos e Referências

Este projeto foi desenvolvido como um exercício prático seguindo o guia do livro:

Livro: Beginning C++ Game Programming
Autor: John Horton
Editora: Packt Publishing
