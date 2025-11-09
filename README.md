# Effect-of-Soil-Type-on-Asparagus-Yield

**📘 Project Overview**
This project investigates how different soil types affect asparagus yield (t/ha).
Using R and the tidyverse ecosystem, the analysis explores yield differences across five soil categories using statistical methods and visualization.

**🎯 Objectives**
Explore asparagus yield data across five soil types.
Perform statistical analysis (ANOVA) to test yield differences.
Visualize yield distribution using ggplot2.
Interpret results to identify which soils perform best.

**🧩 Dataset**
File: asparagus.txt
Variables:
soil: Factor variable (five levels: finest sand, sandy soil, humus sandy soil, claylike sandy soil, sandy clay soil).
yield: Numeric variable indicating yield (t/ha).
Size: 25 observations (5 soil types × 5 replicates)

**🔬 Methods**
Data import and preprocessing
Exploratory analysis (summary stats, boxplots)
One-way ANOVA test
Post-hoc comparisons (Tukey’s HSD)
Visualization and interpretation

**📊 Example Visualization**
Boxplot of yield distribution by soil type:
ggplot(asparagus, aes(x=soil, y=yield, fill=soil)) +
  geom_boxplot() +
  labs(title="Asparagus Yield by Soil Type", x="Soil Type", y="Yield (t/ha)") +
  theme_minimal()
  
**🧠 Key Findings**
The mean yield varies significantly across soil types.
Soils with higher humus content generally produce greater yields.
ANOVA results confirm significant differences (p < 0.05).
