# Roteiro do vídeo: Ir Além (opção 2)

**Duração máxima:** 5 min · **Formato:** gravação de tela com narração · **Publicação:** YouTube, "não listado"

Antes de gravar: deixe `ir_alem/ir_alem_transfer_segmentacao.ipynb` aberto no Colab **já executado**, com todas as saídas visíveis, e a figura do pipeline em `ir_alem/figuras/` aberta em outra aba.

| Tempo | Na tela | O que dizer |
|-------|---------|-------------|
| 0:00 – 0:20 | README, seção Ir Além | "Sou `Leticia Eltermann`, RM `568645`. Neste vídeo mostro a opção 2 do Ir Além: transfer learning com fine tuning e segmentação automática do fundo." |
| 0:20 – 0:50 | Figura do pipeline | Explicar a ideia: primeiro um modelo de segmentação isola o objeto, o fundo é mascarado e só depois a imagem segue para o classificador. |
| 0:50 – 1:30 | Notebook: carga do dataset e motivação | "Com 40 imagens por classe, treinar do zero é frágil. A hipótese é que reaproveitar uma rede pré-treinada e remover o fundo (pasto, céu, galpão) ajuda o modelo a olhar para o que importa." |
| 1:30 – 2:20 | Notebook: segmentação (YOLO-seg/SAM), grade de imagens original, máscara e imagem mascarada | Mostrar exemplos lado a lado. Comentar um caso em que a máscara ficou boa e um em que falhou. |
| 2:20 – 3:10 | Notebook: MobileNetV2, etapa 1 (base congelada) e etapa 2 (fine tuning das últimas camadas) | Explicar por que congelar primeiro e depois liberar algumas camadas com taxa de aprendizado menor. Mostrar as curvas de treino. |
| 3:10 – 4:10 | Notebook: tabela comparativa (CNN do zero, MobileNetV2 sem máscara, MobileNetV2 com máscara) e matrizes de confusão | Dizer o ganho, ou a ausência de ganho, de cada etapa, citando os números da tabela. |
| 4:10 – 4:45 | Notebook: conclusões e limitações | Custo extra de inferência da segmentação, dependência da qualidade da máscara, tamanho pequeno do conjunto de teste. |
| 4:45 – 5:00 | README | "Notebook e figuras estão na pasta `ir_alem` do repositório. Obrigado." |

## Checklist final

- [ ] Duração de no máximo 5 min
- [ ] Nome e RM ditos no início
- [ ] Mostrados: pipeline, segmentação, transfer learning, fine tuning e comparação com números
- [ ] Upload no YouTube com visibilidade **"Não listado"**
- [ ] Link testado em uma janela anônima
- [ ] Link colado no README no lugar de `<LINK_YOUTUBE_IR_ALEM>` e enviado ao GitHub antes do prazo
