# Предсказание уровня удовлетворенности сотрудника и оттока сотрудников
[HTML](https://github.com/Qeecky/Portfolio/blob/main/staff_outflow/staff_outflow.html) [ipynb](https://github.com/Qeecky/Portfolio/blob/main/staff_outflow/staff_outflow.ipynb) <br>
## Описание проекта
Компания предоставила данные с характеристиками сотрудников компании. Среди них — уровень удовлетворённости сотрудника работой в компании. Эту информацию получили из форм обратной связи: сотрудники заполняют тест-опросник, и по его результатам рассчитывается доля их удовлетворённости от 0 до 1, где 0 — совершенно неудовлетворён, 1 — полностью удовлетворён. Необходимо построить модель, которая сможет предсказать уровень удовлетворённости сотрудника на основе данных заказчик и модель, которая сможет на основе данных заказчика предсказать то, что сотрудник уволится из компани.<br>
## Навыки и инструменты
- Python
- pandas
- sklearn.imblearn.Pipeline
- sklearn.model_selection.GridSearchCV
- sklearn.linear_model.LinearRegression, Ridge, Lasso, LogisticRegression
- sklearn.tree.DecisionTreeRegressor, DecisionTreeClassifier
- sklearn.neighbors.KNeighborsClassifier
- sklearn.svm.SVR, SVC
- sklearn.metrics.accuracy_score, roc_auc_score, make_scorer
- sklearn.compose.ColumnTransformer
- sklearn.preprocessing.OneHotEncoder, LabelEncoder, OrdinalEncoder, StandardScaler, MinMaxScaler, RobustScaler
- sklearn.feature_selection.SelectKBest
- imblearn.over_sampling.SMOTE, RandomOverSampler
- imblearn.under_sampling.RandomUnderSampler
- sklearn.impute import SimpleImputer
- shap
- scipy.stats 
- seaborn
- matplotlib
## Общий вывод
В данном проекте были проанализированы данные о сотрудниках компании. Был проведен анализ данных, составлен портрет сотрудника, который хочет уволиться. Было проведено обучение моделей для предсказания уровня удовлетворенности и модель для предсказания ухода сотрудника из компании. Проведена оценка выбранных моделей на тестовой выборке и выбрана лучшая для запуска. Сделаны рекомендации бизнесу

