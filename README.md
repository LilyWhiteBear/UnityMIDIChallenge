# UnityMIDIChallenge
This is the test of **Unity Developer** from **Mutex Team**. Test duration is **7 days** since this test has been received. It is a simple challenge for drawing a gameplay scene from a MIDI file using Unity engine(C#), please thoroughly read before the start.
> Unity engine version 2020.3.14f1

## Requirements
### Gameplay
- The game should contains only a single gameplay screen(no other screens)
- Total 6 note lines

| No. | Note | Sound     | MIDI value | Color  | Score point | Input key |
|-----|------|-----------|------------|--------|-------------|-----------|
| 1   | C#2  | rim snare | 37         | purple | 20          | A         |
| 2   | C#3  | cymbal    | 49         | blue   | 20          | S         |
| 3   | D2   | snare     | 38         | green  | 20          | D         |
| 4   | C2   | bass drum | 36         | yellow | 20          | F         |
| 5   | C3   | high tom  | 48         | orange | 20          | G         |
| 6   | G2   | floor tom | 43         | red    | 20          | H         |

 
- Player must press key on the keyboard in time when the scrolling notes collide with the note indicator
- For every note hit, it should increases the total score by `Score point` from the table
- For every note hit, note should be destroyed/hidden
- When complete a song, player can press `spacebar` to restart the game
- Speed of notes scrolling down is configurable
- Color of notes is configurable
- Size of notes is configurable(optional)
- Score point of notes is configurable
- Input key is configurable

### Game Visual
- Default screen size should be 1270 x 720 with responsive UI
- Displays key panel with input guide(A, S, D, F, G, H) on the bottom of the screen as gameplay screenshots
    - Each key display in its own color (see the color column in the table above)
    - Each key will display key-down feedback
- Displays the note indicator at the top of key panel
- Notes scroll down to the key in vertical in configured speed
    - The notes should be generated by the MIDI data from `DrumTrack1.mid` in `AssetData/Midi`
    - MIDI file is configurable
- Display total score on the top-left of the screen(for example: `Score: 500`)

### Sound
- Play MIDI song in time with scrolling notes using `DrumTrack1.mp3` in `AssetData/Sounds`
    - MIDI song is configurable as the MIDI file

### Additional Requirements
- Unit test is required
- UML Diagram is required, you can use any tools and techniques to create the diagram

## Limitation
- No Playmaker
- 3rd party libraries for **MIDI are allowed**, but others are not
- You can remove/create any files and folders if needed

## Art
- You can use .png file in `AssetData/Sprites` folder to create game sprites
- Game background can be any plain color
- Text can be any font you like

## Evaluation
- Completeness
- Architecture
- Data structures
- Time & memory complexity of algorithms
- Overall Performance
- Code readability
- Code cleanliness
- Unity engine usage
- Design principle, Diagram and Explanation

## Submission
Submit your test by creating PR to this repository
<!-- replace your link here -->
UML diagram: [link](https://viewer.diagrams.net/?tags=%7B%7D&target=blank&highlight=0000ff&edit=_blank&layers=1&nav=1&title=UnityMIDIChallenge.drawio#R7Vtvc6I4HP40zuy9qAMEUF9ubde7me5tp9257r1MIdXcRsJAbPU%2B%2FSUSkCQIaMG67fVN5QdEeJ4nv3%2BJAzBdrmcJjBdfaYjIwLHC9QBcDRzHBmOb%2FxOWTWYZ%2BW5mmCc4lBftDPf4XySNlrSucIhS5UJGKWE4Vo0BjSIUMMUGk4S%2BqJc9UaJ%2BawznyDDcB5CY1gccskVmHXvWzv47wvNF%2Fs22Jc8sYX6xNKQLGNKXkglcD8A0oZRln5brKSICvByX7L4ve84WD5agiLW5AUSryy%2FrZBJsbqw4%2Bvbw3YGzi1E2yjMkK%2FnCCWKrJOK272gZ068wlk%2FPNjkkzyhhmCP0meB5xE2PlDG6HIBLFIWfBeTcRmPET12GMF0g8f12dlryOxZHa8x%2B8M%2BW%2FPy3%2BDycePywQEqcS1lCfxbYi3HMF5dYpHSVBKjmbX0pIJjMEau5zsmuQ6GiDQnrDNElYsmGX5AgAhl%2BVqUCpeLmxXXFrbcU80d2LDk7nJGX3SLnhgN8dYjsQeVdO2r5h9Jj7Exbwg8gf2yQf4dg%2BOm3oxh%2FJDT4%2BQryGknxT0RK7nkkKfbIUofIVGaQYgwE%2FIaBumP3x%2FrRZn8tJ9ezFX6%2Bu%2Fjnwfo%2Bu7ANdj8HjCYGuZywWHxcLUl2AbjM%2Bb6Bj4jc0hQzTBXedUEwGnPrgi2JpJmuGMERmhZe2arjXgyH1rWsyrMapvnhy841A2lalLyyb%2B1XgQL7oTPIxPgrDrGYRagW6Bv8hAQ%2BHJQYJZg%2FDL8eXBFpvt3ZLnlgY5DbEolsQAmBcYoft8MKWBMUrJKUK%2F4OpZl%2F3VrpKgq3vtd6xaxsz4ytUTM2qSliY5kb1%2B2AnMoJ4BnkGJSoIL0sMEP3MdzGkBeez6iaNkGq1URr5C5soHkK18Ru5FdgV4i9c2E7zdjFwnFtv9e7HHhXmpRpwhZ0TiNIymJ%2BpSi7wdtVo%2B6oSqgm1l5fUAMD6m8ieeKpL1yi9qE45eGEFekXH21PeBaXldKwTjk4l8TqYmxVUtwQwruKvGZSPUPcgUOG%2FqQMnTq%2FaktY5auA0xDmqVPS9idD32%2FFmZm%2FWc1j9Zx5AfeXiTyOOlEKz1eOPG6FN7S7cIfV4LUI2%2B8l9BQoNsSeLsJ8NdimqzLALvmgiG5TVqWqL8lU2G8h43hHW4tjAQNdx6CiuhHgyaOrdenU1SY%2FiPjb%2FxjkfQV%2BULpLHO5u2x7l9x3Ga7mfUDvRm92o29KPloTg1SQhr61xtVzdSG5a17hasexYp61xXdNZ3KElfUafUkSeeg20hWyHluep0h259eLlByXPpAraGk78iSrq8WTUIOvtkT7kL5oJuBxA1UsCwDEu%2Fx2ZGYCRpY972rTAMsR6u0oX3PK44jKM2qv1HHL9RiFI1K2h7eZ9zo7TeiMutlWCBxoG2qOE3UD5hfTpKUX9tO98Qy33Im5OKZ%2FslJAP12AaWyppVQ2mquZffw0mu0X29Aapar2cjm21tmyTgC56rZVv4FS4TwI320lhwM7fkanJaYbclBLR4c4z2SdMiGaC0tkGHE9UbobnXniJw1B8TWXRplLXGzeaI%2FQ9g5uqdmFvZYRj9sGvo%2FB%2FZrjzqSioT0qNbS7yGZSUUoeAwDTFgUpQE3RtU8jcX55JFVS02fVq%2FLUrfYVjPNVK3%2BQgjnup4veq4kzI1ual5xzJtTaOrScXPVPtmK1FnpSJPJ8bZ2ewYFAqZD1LKWRtXsSBbgrZtssNbSV4JtpyrIaB%2BhZXi9brYbFi1ySRYpBNkkILBzVJ9gqhceNP6wjVdpPJifp0miDA%2BEhleXqf7sStD8cQllgJ%2B7ClrKt5jLffK2EuQhuUnEsl6xyMtr4g2K6StSe9lUtmTi6mgxD6dBMQM4a%2F79nge%2Bc2G5wWCfXZTIfxoXjr86ES74r5oO%2Bi6M75mOHhjwizN9qIeoIVDjUWH7vB1J949QP1vZ5hBo1i8zhOswBPCK7aCtntFvILa%2BiUs0tr6DruAaWKnS%2Fh7dbc3EnTUnJlqdJDPlvroM5m1U5bUAF6K6VxQWWPpo2Butu6VVkomBXQVbJ5QExs6%2F1gYRk4bxiW634BcGZRuVZHxwblljG5v3rAzIAgYQbc59rMP1zsWkwev%2FGKimuuqDxALBzlKmJY3B7x%2BMr%2FhTiFcYygGWPfDTdadx1UrURWLfz2R05VE%2FZX3HX0jhIQT5%2FARybVI237sDFQz0m1GeMIpeZvMN%2FN5DY2IPfmePnh7se2GV27nyyD6%2F8A)