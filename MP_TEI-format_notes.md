#### Metadata

- [x] Add **"Tagebücher :"** to the document title `/TEI/teiHeader/fileDesc/titleStmt/title` *to allow identification of documents even when separated from DB*.
- [ ] Add the **editors' personnal names** to the `/TEI/teiHeader/fileDesc/titleStmt/editor` *for metadata precision*.
- [ ] Add an AMPI Tagebücher **series** to better connect these TEI-XML files together.

#### Link with DB

- [ ] Declare all **Geovistory entities** in `/TEI/teiHeader/xenoData` : *the sourceDescription element is for the sources from which the document is derived and not to link to another DB.
- [ ] Use **RDF** elements for each entity?
- [ ] Export **entity types**?
- [ ] Export **more structured** data? (With surname, forename, birth and death dates when declared...)? *Useful for static data display.*


#### Referencing entries
- [ ] Correct **Heft numbers**: *all `/TEI/teiHeader/fileDesc/sourceDesc/msDesc` display "Heft 12 (1815-1816) - Anna Maria Preiswerk-Iselin"*.
- [ ] Add a **type** attribute to `//text/body/div` elements with value "eintrag", "stimmung" or "zitat", according to editor's title.
- [ ] Add `#` before each reference.

#### Text
- [ ] Remove "-" before `<lb/>`: *not necessary since `//lb` is here*.
- [ ] Reunite paragraphs when `//pb` in-between and second one starts with a small letter.
- [ ] Make `<add>` elements from text framed by `<>` (with `att.rend='superscript'`).
- [ ] Make `<del>` elements from text framed by `{}` (with `att.rend='strikethrough'`).
- [ ] Make `//del/add` elements when preceding codes are combined (=added, then cancelled).