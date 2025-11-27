# 🏭 Benchmark de Previsão de Produção  

![Dashboard de ROI 800%](download%20(2).png)

*Data-Driven Factory | Machine Learning | ROI 800 %*

&gt; Descobrindo **o que de fato gera mais produção** sem aumentar headcount ou quebrar o caixa.  
&gt; 10 k registros sintéticos → modelos → simulações de custo → **decisão ótima em 3 cliques**.

---

## 1. Visão Geral
Projeto end-to-end que parte de **dados industriais sintéticos** e entrega:
- Ranking de drivers de produção (ex: tempo de ciclo, funcionários, clima).
- Comparação de **investimentos alternativos**: hora extra, contratações ou **melhorias de ambiente**.
- **Modelo Random Forest** com R² = 0,997 e 84 % de acerto dentro de 10 % do valor real.
- **Features de RH** (motivação, fadiga, colaboração) que adicionam 25 % de produção **sem contratar ninguém**.
- **ROI de 800 % e payback de 3 semanas** para o cenário “ambiente interno” – superior a qualquer outro.

---


---

## 3. Resultados-chave
| Cenário | Investimento (R$) | +Produção (un/mês) | Custo/unidade | ROI | Payback |
|---------|-------------------|---------------------|---------------|-----|---------|
| Hora extra | 21 k | 30 | 720 | 80 % | 11 meses |
| +20 % funcionários | 28 k | 188 | 720 | 80 % | 11 meses |
| **Ambiente interno** | **20 k** | **250** | **80** | **800 %** | **3 semanas** |

---

## 4. Modelo & Performance
**Algoritmo:** Random Forest Regressor (100 árvores)  
**Métricas no hold-out (20 %):**
- MAE = 420 unidades
- RMSE = 530 unidades
- R² = 0,997
- Acerto <10 % erro relativo = 84 %

**Top 5 features (importância):**
1. tempo_dias – 0,501
2. quantidade_funcionarios – 0,438
3. dias_trabalho – 0,043
4. temperatura_media – 0,010
5. hora_dia – 0,006

---

## 5. Features Comportamentais (RH)
Incluídas **sem custo adicional** – dados já captados em pesquisas internas.

| Feature | Range | Delta para +1 ponto | Impacto médio |
|---------|-------|---------------------|---------------|
| nivel_motivacao | 1-10 | +1,5 | +5 unidades |
| clima_equipe | 40-100 | +8 | +3 unidades |
| nivel_fatiga | 0-10 | –1,2 | +2 unidades |
| score_colaboracao | 1-10 | +1 | +2,5 unidades |
| horas_treinamento | 0-∞ | — | +1 unidade a cada 4 h |

**Ganho combinado simulado:** +25 % de produção **sem aumentar headcount**.

---

## 6. Economia Final
Produção base = 1 000 unidades/mês
Produção otimizada = 1 250 unidades/mês
Ganho financeiro = 250 × R720=R  180 k/mês
Investimento = R$ 20 k (programas de RH)
ROI = (180 k – 20 k) / 20 k × 100 = 800 %
Payback = 20 k / (180 k / 30) ≈ 3 dias úteis


---

## 7. Entregáveis
- `benchmark_de_previsão_de_produção.py` – script único, 100 % Python.
- CSV `dados_previsao_producao.csv` – base sintética (10 k linhas, 7 colunas).
- 6 gráficos matplotlib/seaborn salvos automaticamente.
- Tabela resumo executiva impressa no console.

---

## 8. Aprendizados
1. **Quantidade de funcionários** não é o único – nem o mais barato – caminho para crescer.
2. **Pequenas melhorias comportamentais** geram efeito similar a contratar 20 % da equipe.
3. **Random Forest** superou linearidade sem perder interpretabilidade (feature importances).
4. **ROI infinito** quando o custo é tempo de gestão, não capital.

---

## 9. Próximos Passos (não executados)
- Substituir base sintética por ERP real.
- Criar API para predição em tempo real.
- Escalar piloto para outras linhas/fábricas.
- Conectar a dashboards Power BI com alertas diários.

---

## 10. Tecnologias
`pandas` | `numpy` | `scikit-learn` | `matplotlib` | `seaborn`

---

**Star ⭐ se 800 % de ROI te fez pensar em ambiente antes de contratar.**
