# 📐 Conscio. Design System (v1.0)

> **"Consistência gera Confiança."**

Este documento define as regras visuais e comportamentais da interface do Conscio.

---

## 1. Tipografia (Typography)

A tipografia equilibra a modernidade com a legibilidade de dados fiscais.

| Função | Família | Pesos | Amostra Visual (Simulação) |
| :--- | :--- | :--- | :--- |
| **Display / Títulos** | `Montserrat` | Bold (700) | **CONSCIO. INTELIGÊNCIA** |
| **Subtítulos** | `Montserrat` | SemiBold (600) | **Serviços Tomados** |
| **Corpo / UI** | `Inter` | Regular (400) | O fim da caça às notas fiscais. |
| **Dados / Código** | `JetBrains Mono` | Regular (400) | `ISS: R$ 145,90` |

> 🔗 **Download:** [Google Fonts: Montserrat](https://fonts.google.com/specimen/Montserrat) | [Google Fonts: Inter](https://fonts.google.com/specimen/Inter)

---

## 2. Paleta de Cores (Color System)

### 🌑 Superfícies (Dark Theme Base)
A base da interface "Deep Petrol" evita a fadiga visual e transmite sofisticação.

| Amostra | Token | Hex | Aplicação |
| :---: | :--- | :--- | :--- |
| ![#0F2027](https://placehold.co/20x20/0F2027/0F2027.png) | `surface-deep` | **`#0F2027`** | **Fundo Global.** Base da janela. |
| ![#182B34](https://placehold.co/20x20/182B34/182B34.png) | `surface-card` | **`#182B34`** | **Cards/Inputs.** Áreas de conteúdo. |
| ![#203642](https://placehold.co/20x20/203642/203642.png) | `surface-hover`| **`#203642`** | **Hover.** Estado ao passar o mouse. |

### ⚡ Marca & Ação (Brand)
Cores vibrantes usadas com parcimônia para guiar a atenção do usuário.

| Amostra | Token | Hex | Aplicação |
| :---: | :--- | :--- | :--- |
| ![#6C5CE7](https://placehold.co/20x20/6C5CE7/6C5CE7.png) | `brand-primary`| **`#6C5CE7`** | **Electric Indigo.** Botões, Links, Logo. |
| ![#5849BE](https://placehold.co/20x20/5849BE/5849BE.png) | `brand-hover`  | **`#5849BE`** | Estado de clique/interação. |
| ![#6C5CE7](https://placehold.co/20x20/6C5CE7/6C5CE7.png?text=+) | `brand-glow`   | *Opacidade* | Efeitos de sombra/brilho (15%). |

### 🚦 Semântica (Feedback)
Cores funcionais para comunicar o status das requisições fiscais.

| Amostra | Token | Hex | Significado |
| :---: | :--- | :--- | :--- |
| ![#00E676](https://placehold.co/20x20/00E676/00E676.png) | `state-success`| **`#00E676`** | **Sucesso.** (Ex: Nota Baixada) |
| ![#FF5252](https://placehold.co/20x20/FF5252/FF5252.png) | `state-error`  | **`#FF5252`** | **Erro.** (Ex: Falha na Prefeitura) |
| ![#FFAB40](https://placehold.co/20x20/FFAB40/FFAB40.png) | `state-warning`| **`#FFAB40`** | **Atenção.** (Ex: Certificado Vencendo) |
| ![#40C4FF](https://placehold.co/20x20/40C4FF/40C4FF.png) | `state-info`   | **`#40C4FF`** | **Info.** (Ex: Processando...) |

### 📝 Texto & Conteúdo

| Amostra | Token | Hex | Aplicação |
| :---: | :--- | :--- | :--- |
| ![#F5F7FA](https://placehold.co/20x20/F5F7FA/F5F7FA.png) | `text-high`    | **`#F5F7FA`** | Títulos e Dados principais (Off-White). |
| ![#A0AAB5](https://placehold.co/20x20/A0AAB5/A0AAB5.png) | `text-medium`  | **`#A0AAB5`** | Labels e Descrições (Cinza Médio). |
| ![#546E7A](https://placehold.co/20x20/546E7A/546E7A.png) | `text-disabled`| **`#546E7A`** | Elementos inativos. |

---

## 3. Componentização & Física (UI Rules)

### Bordas & "Squircles"
Não somos quadrados (velhos), nem redondos demais (infantis).
* **Border Radius Padrão:** `8px` (Inputs, Botões pequenos).
* **Border Radius Cards:** `12px` ou `16px` (Cards grandes, Modais).
* **Conceito:** Suavidade tecnológica.

### Espaçamento (Grid de 4px)
Para manter o alinhamento perfeito, usamos múltiplos de 4.
* **Margens Pequenas:** `4px`, `8px` (distância entre label e input).
* **Margens Médias:** `16px`, `24px` (distância entre elementos internos do card).
* **Margens Grandes:** `32px`, `40px` (distância entre seções).

### Feedback Visual (Affordance)
* **Botões:** Devem ter um estado de *Hover* (mudança de cor) e *Active* (leve "afundamento" ou clique).
* **Loading:** Nunca deixe a interface congelada. Use *Skeleton Screens* (esqueletos cinzas pulsando) ou *Spinners* Roxo/Indigo para indicar processamento.

---

*Este Design System é um organismo vivo. Mantenha-o atualizado conforme o produto evolui.*

---

*© 2026 Conscio Tecnologia.*
