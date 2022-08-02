# Efficient-Autocorrect
Efficient Autocorrect attempts to Split words that are not recognized by autocorrect (spell checker) into largest possible compounds

# Motivation 

no spell checker currently exist that can work for compound words like **studentdesigned,teacherdesigned** etc

note that **studentdesigned** is a compound word that need to be splitted like **'student designed'**
similarly,
**teacherdesigned** should be splitted like **'teacher designed'**
there are many of such misspelled samples exists for what currently no existing english spell checker can work. this implementation attemps to tackle this compound word problem

# compound word splitter

part of this implementation was collected from [compound word splitter ](https://github.com/TimKam/compound-word-splitter) which Splits words that are not recognized by pyenchant (spell checker) into largest possible compounds. these are my contributions
1. replaced pyenchant with nltk and autocorrect instead, because of issues like [this](https://github.com/chiphuyen/sotawhat/issues/7)
2. added better error handlers
3. added contractions fixer
4. preprocessing
5. error analysis demo
