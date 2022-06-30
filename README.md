# wordle
wordle remaining words, best guesses, and optimization

python jupyter notebook with some scratch functions to analyze wordle...
  get possible words matching a given pattern
  pick best next guess
  determine best initial guess

basic idea is to try every legal word and consider every remaining possible answer, and group/count by the resulting pattern (green/yellow/gray combo).
For optimization, find the guess that minimizes the weighted average number of answers under each resulting pattern

conclusion:
using the list of possible answers and legal words from NY Times' version of wordle (available in plaintext on page source),
the best initial guess is 'ROATE' (alternate spelling of 'rote' apparently). It minimizes the expected number of remaining possibilities after 1 and 2 rounds,
and holds whether considering all legal words or only the NY Times answer words
