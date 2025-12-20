# Learning Log

## Why this project exists
I want to understand how agent orchestration frameworks (LangGraph) work in
practice, especially for creative pipelines that require consistency.

## Initial assumptions
- Agents should produce structured outputs
- Images come last
- Reproducibility matters more than creativity

## Open questions
- Where does agent autonomy actually help?
- Where does it hurt?

# Dec 19

## Reflection: Testing Agent prompts
Providing a concrete JSON example dramatically improved field-level compliance.
The model already understood intent; the example resolved ambiguity.

## Reflection: Created first scene illustration
I chose scene 1, the opening scene of the book.  What surprised me most is that the character (Alice) was dressed exactly as I expected (blue dress) and had blond hair, despite not being instructed to do so.  I suspect that the model knows about the popular Disney version of Alice and somehow used that to illustrate the character.  I wonder if the name was different in the prompt if I'd get a very different image.  

### Changing name from Alice to Eliza
ChatGPT confirms that the model uses common depictions of popular characters when ambiguity exists.  Running an experiment to change the character name from Alice to Eliza resulted in character with brown hair and a white dress.  Otherwise the images are quite similar.  

The white rabbit's coat also changes from red to tan.  Sure enough, the Disney character has a red coat.

## Reflection: Creating an image for the second scene
Using the same scene prompt, but changing out the details for the second scene resulted in an acceptable image, but the styling is not quite consistent, nor is the visual depiction of Alice - her hair length and color is changed and she has a white pinafore on in addition to the blue dress.  

## Reflection: Using identity anchoring
Need to add more constraints to get consistency across images.  Adding a character anchor to the character description and an instruction to always include that in the prompt has helped create consistency across scene images.  