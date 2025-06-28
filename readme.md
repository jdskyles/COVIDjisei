# COVID-jisei

_COVID-jisei_ is a poem generator which uses Tracery to create _jisei_, or deathbed poetry, based on the reported final words of those who have died from COVID-19. All poems are in
the haiku form. I used Mark Sample's _Don't Drink the Water_ as a template for this project; below is a bit more info about the updates I made to each of the files, followed by my Process Statement.

## Getting Started

I began by "remixing" my own existing _Obituary_ remix of Mark's project, primarily working with the grammar.js file. I also made some edits to the other files, as described below.

### index.html

I updated the title, button text, and "about" section. Instead of simply rephrasing the button text to "Another poem" or "Another jisei", I decided to emphasize the very personal, human
origin of these words (as well as the ongoing, near-infinite impact of the pandemic - measured person by person) by using the phrase, "Another life lost". Each time the button is pressed, the words on the screen
disappear, never to be recovered, just as the actual voices of the speakers, and the speakers themselves, have disappeared.

### grammar.js

I renamed the variables (and deleted many, which I did not need to use) and filled the arrays with my own data. 
I found that I needed to embed variables within variables, to allow for the different combinations that could add up to the correct
number of syllables for each line. For example, a seven-syllable line could contain text from an array with seven-syllables, or from two arrays, one with five-syllables and the other 
with two syllables (and five syllables may also be created from the three- and two-syllable arrays).  The order of selection from these arrays could also vary. To allow for an equal probability of
selection from all of the possible line options, I listed the five- and seven-syllable arrays multiple times, equal to the number of other options for each line.

### style.css

I center-justified all text, updated the font to EB Garamond, and changed the background and font colors to better complement my project's theme.
I also increased the spacing between the elements on the page, since each poem is only three lines in length.

### Assets

I did not modify this file (the assets remain empty). I felt that simply the text, without any accompanying images, is most appropriate and effective.

### Other Files

I did not modify the tracery.js file.

### Process Statement

During our class, I had originally begun remixing Mark’s _Don't Drink the Water_ code into one that would generate obituaries.  When I later read the 
assignment for this week and considered serious topics that would “tell a story”, and the need for a very large number of possible outputs, I started 
thinking about the concept of "last words" and the incredibly large number of lives lost due to COVID-19 in the past two years. A bit of online research led 
me to an article about the loss of these patients' last words, as many die alone and/or are on ventilators, so are unable to speak. I have, however,
read about the final words of these patients before they are intubated.  It occurred to me that these are truly their "last words", and could be presented
in the format of a jisei, or Zen deathbed poem.  These are typically haiku or tanka that are composed on one's deathbed, shortly before 
dying, and are said to be one's truest statement.  I decided to design a poetry generator which would create haiku by blending together the final words of 
those who died from COVID-19.  To do so, I found news articles where nurses or loved ones provided direct quotes (or copies of 
letters/texts) from the patients.  I've included below all of the links to the articles I've utilized.  I've also included links to articles which helped to shape
my thought process and self-reflection on the meaning behind such a project, the possible reasons for my own interest in the topic, and how I could honor
and maintain the dignity of the patients whose words I incorporated.

In order to ensure I was not only meeting the 5-7-5 syllable count for each line, but also creating grammatically correct sentences, I discovered that I needed 
to think very carefully about how I organized and populated my arrays.  I found that it was easiest to create groupings of seven syllables, five syllables, three 
syllables, and two syllables.  Then the seven and five syllable groups could be used directly, or lines could be built using a combination of the two, three, and 
five syllable groups.  I also needed to be careful which words I used to open and close each individual option in the arrays, as I wanted to ensure there would be
a grammatically correct flow both within and between the lines of the haiku, while remaining true to the apparent meaning of the original speaker.  Some quotes worked
best as shorter sections, even as one word, whereas others would lose meaning or grammatical "fit" if reduced.  And in many cases the meaning of the quote could easily
be changed (or even become its opposite) if reduced too much... for example, "I thought this was a hoax" vs. "this was a hoax". Yet despite these efforts, I still found
that the randomized juxtaposition of the lines could also alter their meaning, which was an interesting lesson in how flexible and context-dependent language can be,
and how easily misunderstandings can arise. This then is itself an example of how politicized, mis-interpreted, and often conflicting information has circulated throughout
the pandemic. 

I also found it interesting, although not quite surprising, that the gender of the words is primarily female ("mom", "mama", "daughter", "girl"). Fathers and sons do not 
make any appearance.  This seems to reflect our patriarchal society and culture in general, where those dying are known to call out for their mothers (the typical caregivers)
while female family members (wives and daughters) are still thought to be under the care of their male relatives. I am aware that biological males have been dying of COVID-19 
at higher rates than females, but I have more equally used the words of male- and female-identified patients (six and five, respectively) for the poems.

In creating my code, I considered adding arrays with four-syllable and six/one-syllable options, but found that there were not many source texts that would support this length
while still creating lines that were true to the speaker's intent and a grammatical fit with the other lines (for instance, options of this length would often need to start
or end with prepositions or modifiers). Perhaps as would be expected, those who are severely ill and struggling to breathe spoke in shorter, monosyllabic statements, or instead
had written their final words, creating longer, multi-syllabic texts.  Thus, groupings of seven, five, three, and two syllables seemed to work best.  I also quickly 
discovered that the options in the two-syllable array would repeat more frequently in the poems, as they are an option in all three of the lines, plus these options are 
shortened repetitions of the existing longer lines. Therefore, I tried to ensure that the options in the two-syllable array were ones that actually did repeat between the various 
different speakers, or touched on common themes.

I did not really encounter any errors when creating my code, as it is rather simple and straightforward.  However, I did find myself frequently adding or removing words, thus 
changing the number of syllables in each option, for the reasons mentioned above.  I also occasionally missed a quotation mark or comma, which I then needed to go back and add in 
order for the code to run.

The original code I was using as a template had grey text on a white background and a more business-like font.  To reflect the seriousness and poignancy of the words, along with the 
connection to death, I found that a black background with white text was more appropriate and very striking.  Similarly, I wanted to use a font that would be less mechanistic and 
more reflective of the personal, intimate words in the source texts, so I selected EB Garamond, which is quite sparse but with a rounded softness to the letters.  I really liked the 
grey to red highlighting of the button when one hovers over it, so decided to keep that.  I did increase the spacing between all of the elements on the page and center-justified 
everything, for readability and to maintain that simple, sparse feel.

I am very happy with the results of my efforts, and continually find myself quite moved, even tearing up, as I read some of the resulting haiku.

_Articles which guided my thought process:_ <br>
[The Tragic Loss of Coronavirus Patients’ Final Words](https://www.theatlantic.com/health/archive/2020/07/covid-dying-words/613951/)<br>
[Wikipedia: Jisei](https://en.wikipedia.org/wiki/Death_poem)<br>
[The Chilling Popularity of Anti-Vax Deathbed Videos](https://newrepublic.com/article/163666/covid-unvaccinated-deathbed-videos)<br>

_Origin of dataset/reported final words of COVID patients:_ <br>
[Son's haunting last words to mum before dying from COVID](https://au.news.yahoo.com/sons-haunting-last-words-to-mum-before-dying-from-covid-111817947.html)<br>
[A nurse revealed the tragic last words of his coronavirus patient](https://www.cnn.com/2020/04/11/health/nurse-last-words-coronavirus-patient-trnd/index.html)<br>
[Dying of COVID-19, she called the newsroom to share her last words](https://www.wbir.com/article/news/health/coronavirus/woman-dying-of-covid-gives-last-words/51-9cff3909-a051-41ce-97b2-c50b222eb702)<br>
[Son shares heartbreaking account of mother’s last words as she battled COVID-19](https://www.wavy.com/news/health/coronavirus/son-shares-heartbreaking-account-of-mothers-suffering-last-words-as-she-battled-covid-19/)<br>
[20-Year-Old With COVID-19 Uses Last Words to Tell Mother She Doesn’t Want to Die](https://www.complex.com/life/20-year-old-covid-19-last-words-tell-mother-doesnt-want-to-die/)<br>
[The Heartbreaking Last Texts of a Hospital Worker on the Front Lines](https://www.nytimes.com/2020/04/15/nyregion/coronavirus-woodhull-madhvi-aya-dead.html)<br>
[Nurse sends Valley family reassuring video message hours before losing his life](https://abc30.com/mexico-nurse-madera-last-words-video-message/7883838/)<br>
[Family shares last moments after vaccinated San Antonio mother dies from COVID-19](https://www.kens5.com/article/news/local/i-cant-breathe-family-share-last-moments-after-vaccinated-san-antonio-mother-dies-from-covid/273-3bb89d53-0db4-462c-9556-8341161c0d5c)<br>
[ICU nurse delivers mother’s last words](https://www.kxly.com/tell-my-daughter-i-love-her-icu-nurse-delivers-mothers-last-words/)<br>
[A couple died of COVID, leaving five children behind](https://www.washingtonpost.com/nation/2021/10/21/stafford-virginia-couple-die-covid-19/)<br>
[Lee County father’s last words on COVID death bed](https://abc-7.com/news/2021/03/03/lee-county-fathers-last-words-on-covid-death-bed-take-care-of-my-girl/)<br>
