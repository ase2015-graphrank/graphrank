There are five folders in this dataset and each folder contains dataset for an open source software project.


benchmark.txt:

50 lines. Each line contains a question id.

To access this benchmark question, we can visit stackoverflow.com/questions/{question_id}


posts.txt:

all relevant posts for this project we crawled from StackOverflow.

Each post takes up three lines:

Line 1 contains the corresponding question id;

Line 2 contains the text content of the title and the question, all space characters are formalized to " ";

Line 3 contains the text content of answers and comments.


rank.txt and ir-rank.txt:

the position the answers are ranked.

Each benchmark question takes up a line, which contains two numbers.

The first number is the question id, and the second number is the position the corresponding answer is ranked.


suggestion.txt and ir-suggestion.txt:

suggested posts for each benchmark question.

Each line contains several numbers.

The first number is the question id, and the following numbers are the ranked list of question ids.


rank2.txt:

manual labels, only for lucene and jfreechart.

Each line contains tree numbers.

The first number is the question id;

The second number is the position of the first helpful post in the list suggested through graphrank.

The third number is the position of the first helpful post in the list suggested through the baseline.

Notice that in the list, the "new" post is removed.
