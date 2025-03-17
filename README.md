# Conceitos Essenciais sobre a biblioteca Pandas

## 1. Fundamentos do Pandas
- ✅ **O que é o pandas e para que serve**: Biblioteca Python para manipulação e análise de dados estruturados.
- ✅ **Diferença entre Series e DataFrame**: Series é uma estrutura unidimensional semelhante a um array, enquanto DataFrame é uma tabela bidimensional com colunas e linhas.
- ✅ **001. Como instalar e importar o Pandas**: `pip install pandas` e `import pandas as pd`.

## 2. Estruturas de Dados do Pandas
- ✅ **002. Series**: `pd.Series()`, `s.values`, `s.index`, `s.dtype`
- ✅ **002. DataFrame**: `pd.DataFrame()`, `df.values`, `df.columns`, `df.dtypes`
- ✅ **003. Indexação e rótulos**: `df.index`, `df.set_index()`, `df.reset_index()`

## 3. Carregamento de Dados
- ✅ **004. Leitura de arquivos**:
  - `pd.read_csv()`, `pd.read_excel()`, `pd.read_json()`, `pd.read_sql()`, `pd.read_parquet()`
- ✅ **004. Escrita de arquivos**:
  - `df.to_csv()`, `df.to_excel()`, `df.to_json()`, `df.to_sql()`, `df.to_parquet()`

## 4. Manipulação de Dados
- ✅ **005. Seleção de colunas e linhas**: `df['coluna']`, `df[['col1', 'col2']]`, `df.loc[]`, `df.iloc[]`, `df.at[]`, `df.iat[]`
- ✅ **006. Filtragem de dados**: `df[df['coluna'] > valor]`, `df.query()`
- ✅ **007. Adição, remoção e modificação de colunas**: `df['nova_coluna'] = valores`, `df.drop(columns=['coluna'])`, `df.assign()`
- ✅ **008. Ordenação de dados**: `df.sort_values(by='coluna')`, `df.sort_index()`
- ✅ **009. Reset e configuração de índice**: `df.reset_index()`, `df.set_index('coluna')`

## 5. Operações e Transformações
- ✅ **Aplicação de funções**: `df.apply()`, `df.map()`, `df.applymap()`
- ✅ **Manipulação de strings**: `df['coluna'].str.contains()`, `df['coluna'].str.replace()`, `df['coluna'].str.extract()`
- ✅ **Tratamento de valores nulos**: `df.isna()`, `df.fillna()`, `df.dropna()`
- ✅ **Substituição de valores**: `df.replace()`
- ✅ **Agrupamento de dados**: `df.groupby()`, `df.agg()`
- ✅ **Pivotamento e transposição**: `df.pivot()`, `df.melt()`

## 6. Análise Estatística e Agregações
- ✅ **Estatísticas descritivas**: `df.mean()`, `df.median()`, `df.std()`, `df.describe()`
- ✅ **Contagem de valores**: `df['coluna'].value_counts()`
- ✅ **Operações matemáticas e estatísticas**: `df.sum()`, `df.cumsum()`, `df.min()`, `df.max()`
- ✅ **Aplicação de funções personalizadas**: `df.agg()`, `df.applymap()`

## 7. Trabalhando com Datas e Horas
- ✅ **Conversão de strings para datas**: `pd.to_datetime()`
- ✅ **Extração de informações**: `df['data'].dt.year`, `df['data'].dt.month`, `df['data'].dt.day`
- ✅ **Operações com datas**: `pd.Timedelta()`, `pd.date_range()`

## 8. Mesclagem e Combinação de Dados
- ✅ **Junção de DataFrames**: `pd.merge()`, `df.join()`
- ✅ **Concatenação de DataFrames**: `pd.concat()`
- ✅ **Merge types**: `how='inner'`, `how='outer'`, `how='left'`, `how='right'`

## 9. Trabalhando com Dados Faltantes e Duplicados
- ✅ **Identificação e remoção de valores nulos**: `df.isna()`, `df.dropna()`
- ✅ **Preenchimento de valores**: `df.fillna()`
- ✅ **Identificação e remoção de duplicatas**: `df.duplicated()`, `df.drop_duplicates()`

## 10. Visualização de Dados com pandas
- ✅ **Geração de gráficos**: `df.plot()`, `df.hist()`, `df.boxplot()`, `df.bar()`, `df.scatter()`
- ✅ **Integração com Matplotlib e Seaborn**: `import matplotlib.pyplot as plt`, `import seaborn as sns`

## 11. Trabalhando com Dados Categóricos
- ✅ **Conversão de colunas para tipo category**: `df['coluna'].astype('category')`
- ✅ **Manipulação de categorias**: `df['coluna'].cat.codes`, `df['coluna'].cat.categories`

## 12. Otimização e Desempenho
- ✅ **Uso de tipos de dados eficientes**: `df.astype()`
- ✅ **Uso de Parquet e Feather**: `df.to_parquet()`, `df.to_feather()`
- ✅ **Uso de chunks para grandes volumes de dados**: `pd.read_csv(chunksize=n)`

## 13. Pandas Avançado
- ✅ **Expressões Regulares em pandas**: `df['coluna'].str.extract()`, `df['coluna'].str.findall()`
- ✅ **Manipulação de JSON e APIs**: `pd.json_normalize()`
- ✅ **Trabalhando com MultiIndex**: `df.set_index([col1, col2])`, `df.stack()`, `df.unstack()`
- ✅ **Trabalhando com Janela Móvel**: `df.rolling()`, `df.expanding()`