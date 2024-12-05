import pandas as pd

# Estrutura do cronograma
data = {
    "Horário": [
        "08h00 – 08h50",
        "08h50 – 09h40",
        "09h40 – 10h00",
        "10h00 – 10h50",
        "10h50 – 11h40",
        "11h40 – 12h30",
        "14h00 – 14h40",
        "14h40 – 15h30",
        "15h30 – 15h50",
        "15h50 – 16h40",
        "18h em diante"
    ],
    "Atividade": [
        "Tema Administrativo (teoria ou leitura aprofundada)",
        "Matemática (exercícios e revisões de conceitos)",
        "Intervalo (lanche leve, alongamento)",
        "Português (interpretação de texto ou gramática)",
        "Graduação/Pós (revisão de aulas ou leitura de materiais)",
        "Simulados ou questões de concursos (temas mistos)",
        "Revisão do que foi estudado pela manhã (uso de flashcards ou resumos)",
        "Neurociência (leitura ou trabalhos da pós)",
        "Intervalo (pausa para descansar a mente)",
        "Prática: questões de concursos ou elaboração de resumos/mapas mentais",
        "Lazer e Relaxamento (hobbies, séries, leitura leve)"
    ]
}

# Criar DataFrame
df = pd.DataFrame(data)

# Salvar como arquivo Excel
file_path = "/mnt/data/Cronograma_de_Estudos.xlsx"
df.to_excel(file_path, index=False, sheet_name="Cronograma")

file_path
