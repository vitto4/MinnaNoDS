
# 🗳️ Opinions

- In each lesson, words are ordered like they are in the second edition. <br>
  As such, words that are only present in the first edition are placed at the very end of the lesson, marked by the comment :
  ```yaml
    # ------------------------------------ ED1 ----------------------------------- #
  ```
  In such sections, words appear in the same order as they do in the first edition.
- In some cases, the same word is present in both the first and second editions, but with different translations. <br>
  In such cases, I kept the version from the second edition. However, when it felt like both versions were helpful in understanding the word, I may have :
    - Combined the two. This is indicated with comments using the syntax. <br>
      ```yaml
      # !MOD KEPT <short description here>
      ```
      Where `!MOD` stands for « modification ».
    - Went « i'll just deal with it later 👍 » (spoiler : I didn't) <br>
      ```yaml
      # ?ADD `<meaning present in edition one, that may be added to the one from edition two, or may sit in this comment forever>`
      ```
- Occasionally the books contain spelling or grammar mistakes. They may be rectified when they can be definitively categorized as mistakes, and there is an obvious correction to be made. In that case, it is indicated by a comment :
  ```yaml
  # !MOD REPLACED : `<word with typo>` --> `<corrected version>`
  ```
- `Minna no Nihongo`-specific vocabulary (like `IMC／パワー電気／ブラジルエアー`) is included.
- Formatting rules were decided arbitrarily, I chose what looked or sounded best to me. If you find one of these rules is broken somewhere, don't hesitate to report it through an issue.
  <div align="center">
  <details>
    <summary>The rules <sub><sup><sub><sup><sub><sup><sub><sup><sub><sup>are simple</sup></sub></sup></sub></sup></sub></sup></sub></sup></sub></summary>
    <div align="left">

    - When a word has no `kanji`, the field is set to null using a `~`.
    - In fields `kanji` and `kana` :
      - Regular spaces ` ` are used over ideographic spaces `　`. <br>
        Example : `～から 来ました。`.
      - Fullwidth parentheses `（` and `）` are used. No space should be inserted before nor after. <br>
        Example : `だれ（どなた）`.
      - Fullwidth square brackets `［` and `］` are used. No space should be inserted before nor after. <br>
        Example : `［どうぞ］よろしく［お願いします］。`.
      - Fullwidth tildes `～` are also invited to the party, and they may be used in combination with spaces. <br>
        Example : `この ～`, `撮ります［写真を～］`.
      - Ideographic full stops `。` and ideographic commas `、` shall also be used ; as usual with no trailing space. <br>
        Example : `じゃ、また［あした］。`.
      - Fullwidth numbers are used over *basic latin* ones. <br>
        Example : `１日` instead of `1 日`.
      - Use the fullwidth solidus `／` instead of the solidus `/`. <br>
        Example : `さくら大学／富士大学`.
    - In `meaning` :
      - Prefer regular parentheses `(` and `)` as well as regular square brackets `[` and `]`, except when a string in Japanese is inserted. <br>
        Example : `put on [glasses]` or `Pleased to meet you, too. (response to［どうぞ］よろしく［おねがいします］。)`. Notice the regular parentheses enclosing the Japanese part, with fullwidth square brackets inside.
      - Use fullwidth tildes `～` and fullwidth hyphen-minuses `－` when necessary. <br>
        Example : `I'm from ～ (country)`, `－ years old`.
      - Regular colons `:` (may be enclosed in spaces) are used instead of fullwidth colons `：`. <br>
        Example : `meeting, conference (～を します : hold a meeting)`.
      - Regular solidi `/` are preferred. <br>
        Example : `You're welcome./Don't mention it.`.
      - Regular apostrophes `'` are preferred. <br>
        Example : `That's good.` and `'The Seven Samurai', a classic movie by Akira Kurosawa`.
      - Add spaces around French guillemets. <br>
        Example : `froid (le temps «il fait froid»)` --> `froid (le temps « il fait froid »)`.
      - For languages such as French that require a space before punctuation, replace `*:` by <code>&nbsp;:&nbsp;</code> but keep `*?` and `*!`. <br>
        Example : `Oui?` is kept this way ; but edit `football (～を します:jouer au football)` into `football (～を します : jouer au football)`.
      - When a meaning is missing from the database, it is set to `null`. <br>
        Example : `fr: null,`.
    </div>
  </details>
  </div>