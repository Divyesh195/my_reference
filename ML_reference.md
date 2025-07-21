# Machine Learning basic code


1. Remove columns with null data

> data = data.dropna( axis = 1, how="all")

*how takes only two values 1. ALL = drops row/column if all entries are null   2. ANY = drops row/column is any entry is null. 

<hr>

2. Train test splitting :

> from sklearn.model_selection import train_test_split

> X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size = 0.2, random_state = 42, shuffle = true)

<hr>

3. To count categorical values in column

> data['column_name'].value_counts()