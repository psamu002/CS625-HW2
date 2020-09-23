HW2
================
Paul Samuel
9/22/2020

\*\*Here are high level activities I performed for data clean up: 1.
Cleaned up type of pet using all the options “Cluster Edit”. Here are
details: key collision/fingerprint –\> - dog, Dog., dog :))))) to Dog -
cat, Cat\! to Cat  
\- Guinea pig to Guinea Pig - bunny to Bunny - hamster to Hamster -
Hermit crab to Hermit Crab key collision/ngram-metaphone3/Ngram Size 1 -
Doggo, God –\> Dog - Beta fish –\> Betta fish key
collision/cologne-phonetic - Cats, Katze –\> Cat - Rabbit, Robot –\>
Bunny - Dig –\> Dog key collision/Diatch-Mokotoff - Phoebe, Puppy –\>
Dog key collision/Beider-Morse Cats, Ca –\> Cat nearest
neighbor/levenshtein/radius 1/chars 2 Car –\> Cat

2.  After performing cluster edit on type of pet, i performed Text Facet
    and manually reviewed and made needed edits

<!-- end list -->

  - Betta Fish –\> Fish and Updated breed to Betta Fish
  - Car –\> Cat
  - Replaced following with null using edit cells/transform: (Other),
    Other , Other-, Other: to remove other
  - Used edit cells/common transforms/To titlecase to have consistency
    so things like guinee pig gets corrected
  - Updated manually (fish) to Fish
  - Used edit cells/common transforms/Trim leading and trailing white
    space
  - Used edit cells/split multi-valued cells to split record that had
    multiple entries
  - Used edit cells/common transforms/Trim leading and trailing white
    space
  - Manually - dlg –\> Dog
  - Goldfish –\> Fish and Updated breed to Gold Fish
  - Indoor Goldfish –\> Fish and Updated breed to Gold Fish
  - Kitten & Kitty Meow to Cat
  - Luna & Mona to Dog
  - Car –\> Cat
  - Pit bull –\> Dog
  - Blank to Dog
  - Sog to Dog
  - Deleted Roomba, server, virus, blank, card board poster using
    All/Edit row/Remove matching rows

<!-- end list -->

3.  Cleaned up Breeds similar to type of pet using cluster and edit and
    manual edits key collision/fingerprint –\>

<!-- end list -->

  - 6 combos of Golden Retriever and 87 other clusters key
    collision/ngram-metaphone3/Ngram Size 2
  - 16 clusters key collision/ngram-metaphone3/Ngram Size 1
  - Selectively changed few key collision/cologne-phonetic
  - Selectivley changed few key collision/Diatch-Mokotoff
  - Selectivley changed few key collision/Beider-Morse
  - Selectivley changed few nearest neighbor/levenshtein/radius 1/chars
    2
  - Selectivley changed few
  - Removed spaces
  - Changed titlecase

4.Cleaned up pets age using cluster and edit and manual edits

Questions and Answers:

1.  How many types (kinds) of pets are there?

2.  How many dogs?

3.  How many breeds of dogs?

4.  What’s the most popular dog breed?

5.  What’s the age range of the dogs? What’s the age range of the guinea
    pigs? What is the oldest pet? Which are more popular, betta fish or
    goldfish? How many of each? What’s the most popular everyday name
    for a cat? What’s the most popular full name for a dog?

Cleaned up File Name: HW2-petnames.csv All activities performed for
clean up are available in JSON file: HW2-petnames.json

*This text is Italics.* **This is bold text** ***This is bold and
italics***

![](Images/PetCount.png)