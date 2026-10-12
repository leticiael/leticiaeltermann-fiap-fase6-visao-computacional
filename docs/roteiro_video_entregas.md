# Roteiro do vídeo: Entregas 1 e 2

**Duração máxima:** 5 min · **Formato:** gravação de tela com narração · **Publicação:** YouTube, "não listado"

Antes de gravar: deixe o notebook principal aberto no Colab **já executado** (todas as saídas visíveis), a pasta do Drive aberta em outra aba e o Make Sense com o projeto carregado em uma terceira aba. Não rode treinamentos durante a gravação.

| Tempo | Na tela | O que dizer |
|-------|---------|-------------|
| 0:00 – 0:20 | README no GitHub, com a figura de arquitetura | "Olá, sou `Leticia Eltermann`, RM `568645`. Este é o projeto da Fase 6: a FarmTech Solutions quer mostrar a um cliente do agronegócio que dá para detectar vacas e tratores em imagens com visão computacional." |
| 0:20 – 0:50 | Figura de arquitetura (zoom) | Percorrer o fluxo: coleta, organização no Drive, rotulação no Make Sense, três modelos no Colab, avaliação e inferência. |
| 0:50 – 1:20 | Pasta `MyDrive/fiap_fase6/dataset` no Drive e `dataset/CREDITS.md` | "São 40 imagens por classe, divididas em 32 de treino, 4 de validação e 4 de teste. Todas vêm de fontes com licença aberta, com os créditos registrados." |
| 1:20 – 1:50 | Make Sense com algumas imagens rotuladas | "Rotulei cada imagem com caixas delimitadoras e exportei no formato YOLO, com as classes 0 vaca e 1 trator." |
| 1:50 – 2:40 | Notebook: seção do YOLOv5 customizado, gráficos de treino e tabela de métricas de 30 e 60 épocas | Comparar as duas simulações: mAP, precisão, recall e perdas. Dizer qual configuração ficou melhor e por quê. |
| 2:40 – 3:05 | Notebook: imagens de teste com as caixas previstas | "Aqui está o modelo vendo imagens que ele nunca viu no treino." Comentar um acerto e um erro, se houver. |
| 3:05 – 3:35 | Notebook: YOLOv5s padrão (COCO) | "O modelo padrão já conhece 'cow' e 'truck', mas não 'trator'. Vejam o que ele faz com as mesmas imagens." |
| 3:35 – 4:05 | Notebook: CNN do zero (curvas e acurácia) | "A CNN treinada do zero só classifica a imagem inteira, não localiza o objeto, e com tão poucas imagens tende a sobreajustar." |
| 4:05 – 4:45 | Notebook: tabela/gráfico comparativo final | Comparar as três abordagens em facilidade de uso, precisão, tempo de treino e tempo de inferência. Dizer qual é recomendada ao cliente. |
| 4:45 – 5:00 | README no GitHub | "O link do notebook e os detalhes estão no README. Obrigado." |

## Dicas de gravação

- Ensaie uma vez cronometrando; corte falas em vez de acelerar.
- Use zoom do navegador em 125–150% para que tabelas e gráficos fiquem legíveis.
- Feche abas e notificações que não fazem parte do roteiro.

## Checklist final

- [ ] Duração de no máximo 5 min
- [ ] Nome e RM ditos no início
- [ ] Mostrados: dataset, rotulação, YOLO customizado (30 e 60 épocas), YOLO padrão, CNN do zero e comparação
- [ ] Upload no YouTube com visibilidade **"Não listado"**
- [ ] Link testado em uma janela anônima
- [ ] Link colado no README no lugar de `<LINK_YOUTUBE_ENTREGAS>` e enviado ao GitHub antes do prazo
