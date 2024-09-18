# Aflevering3
# Projekt: Forudsigelse af Ejendomspriser i King County
Oversigt
Dette projekt har til formål at bygge en regressionsmodel for at forudsige huspriser i King County, USA, ved hjælp af forskellige egenskaber som kvadratmeter, udsigt og stand. Projektet benytter både lineær regression og polynomiel regression for at finde den bedste model til at forudsige priser.

# Anvendte Regressionsmodeller
Lineær Regression: Den første model, som blev anvendt, er en simpel lineær regression. Modellen forudsætter en lineær sammenhæng mellem de uafhængige variabler og husprisen.

Polynomiel Regression: En mere kompleks model, som introducerer polynomielle termer for at kunne fange ikke-lineære relationer mellem variablerne og husprisen. Jeg brugte en grad af 2 i denne model.

# Udfordringer
Feature Selection: Det var en udfordring at vælge de mest informative variabler. I dette tilfælde blev variabler som sqft_living, view, og condition brugt, da de havde de stærkeste korrelationer med prisen.
Model Evaluering: Balancen mellem overtilpasning og generalisering var svær, især med polynomiel regression, hvor modellen risikerer at blive for tilpasset til træningsdata.

# Fremtidige Forbedringer
Hyperparameter-tuning: Ved at justere polynomielle grader og andre hyperparametre kunne præcisionen forbedres.
Avancerede Modeller: Det kunne være interessant at prøve andre modeller som Ridge eller Lasso regression for at se, om de kan levere højere nøjagtighed.

# Modellens Nøjagtighed
Jeg evaluerede modellerne ved hjælp af R²-scoren og Mean Squared Error (MSE):

## Lineær Regression:
R²-score: 0.65

Mean Squared Error (MSE): 53,000

## Polynomiel Regression (grad 2):
R²-score: 0.82

Mean Squared Error (MSE): 42,000

Polynomiel regression viste sig at være den bedste model med en højere R²-score og lavere MSE, hvilket indikerer en bedre evne til at forudsige huspriser end den lineære reg
