# WDBasics

HTML header elements (blocks of website header text) are bracketed by <h1> and </h1>. The number that follows the H denotes the position on the page, with 1 being the highest and going from there.

Web page paragraphs are created using <p></p>.

A comment is a message that appears in the HTML code but does not appear on the finished web page. You can create these with <!-- and end them with -->

You can enclose different 'content areas' of a web page using certain elements. To specify the "main" part of the page, you would use <main> </main>. Putting multiple other elements inside one of these content areas is called nesting. When creating sub-sections, you can use <section> instead of <main>, and you ought to stick with h2 or lower heading elements to indicate these are sub-sections.

You can tell when elements within coding are nested, as they'll be placed about two spaces right of the nest element. So the h1, p, and the comment you created inside <main></main> should show as being two spaces further than the start and end of <main>

The <img> element is known as a self-closing element, because you don't need to provide an end point like you would with h1 or p.

Attributes are special words added inside an element that can control how it behaves. For img, an src attribute can be added to specify a URL where the image desired can be found. In this case the URL would be added like this: <img src="https://www.example.com/the-image.jpg">

<img> elements should be created with an alt attribute too, which dictates the text that will show if an image cannot be loaded properly. This would be added as alt="image was here"

The anchor element <a> can be used to link to another web page. An example would be <a href='https://google.com'>Click here to go to Google.com</a>  - Note that after the first end bracket, the text of the hyperlink is written, which will show on the web page.

You can also add an anchor element inside another element, such as placing it around words within header text blocks or within a paragraph. The same format as above would be used, just partway inside another element string.

To make the hyperlink open in a new tab, which is standard for most sites, another element should be added directly after the website address in the <a> element string. This is target="_blank". Note this should be before the first closing bracket.

You can also place an anchor around an image string, just ensuring that where the text would normally be, you include both the image location and the alt string. An example would be as follows: 

<a target="_blank" href="https://google.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>

In the above, the target website is Google, the image is a free image of a cat, and the text replacing the image is written right before the </a> element to close the anchor.

The element <ul> can be used to designate an unordered list. Within the <ul> string, the element (there can be multiple) of <li> can be used to designate individual list items.

Figure elements can be used to designate self-contained content, and will allow images to be captioned. The caption is added using <figcaption> after the img but within the nest of the figure element.

You can wrap words inside the <em> element to emphasise them in a text string. You can likewise indicate emphasis using <strong>. em is italics, while strong is bold.

The element <ol> is used to create an ordered, or numbered, list.

The <form> element can be used to create a web form on a site. The action attribute can then be added to indicate where form data should be sent, in the format <form action="WEBSITE"></form>

Having established where the data will be sent, the self-closing <input> element allows data to be collected from the web form. Adding the type= attribute allows customization of the input, such as in <input type="text"> to allow text input from a user. The designation 'required' can be added after the word input to ensure users cannot submit until all relevant info has been provided.

You can also add a name field with name= after the type has been designated, and give users a hint about what to enter using placeholder=, again after the type.

<button> can be used to create a clickable button. When linked to form, the default action of a button is to submit the form to the location specified earlier. You can rename a button by adding a type element to the first bracket, such as <button type="Button Name"> Submit</button>

Some elements, such as <input> and <button>, are inline elements. This means even if the code for them is on separate lines, they will occupy the same line on the web page.

You can use radio buttons, which are alike to bullet points, to allow users to select one or several specific answers instead of typing into a text box. These are created using <input type="radio"> TEXT. You can also nest this element inside <label></label>, this means clicking the word TEXT would also activate the button - useful for screen readers.

To make it so that selecting one radio button will de-select another, all radio buttons in sequence must have an identical name= attribute. Example name="radio button list". Adding a name attribute to inputs can also help processing time for a server, especially with multiple inputs.

The id attribute can be used to give a piece of HTML code a specific "name" that must be unique from any other id used elsewhere. This is done via id="text". 

Data submitted for a form includes both the name and value attributes. Name as mentioned above indicates the group the buttons belong to, but value can specify which button exactly was selected. Because of this, a value= attribute should be unique, similar to id, and infact it can be the same as the id. 

<fieldset> allows inputs and labels to be nested together within a web form. You can also add a <legend> element to create a caption for the whole fieldset, which can be used to indicate to users what they ought to include in the form.

The third input type is type="checkbox", which allows the user to check a box. This can be used the same way as radio buttons. As best practice, both name and value attributes should be included as with the radio button example.

You can use a for= attribute to indicate that an element should be linked with another element, specifically by making the for= the same as the id of the target element. You would nest a for attribute inside a label element.

You can make either a radio or checkbox input selected by default, simply be adding the attribute checked to the input. No value needs to be assigned to checked, just add the word.

While content for a web page goes into the <body> element, the <head> element is used to contain other useful information that will not be rendered.

One example of head content is <title>, which determines what browsers will show in the title bar or tab for the web page.

All elements we have discussed will be encompassed by an html element, which acts as the nest for all the information on a page. You can add a lang element to this element to specify the language of the page (e.g. - en for English). On the line just prior to html, all pages should also hold the special string <!DOCTYPE html>. The self-closing <meta charset="UTF-8"> can also be added to the head, to allow browser to parse the page into multiple languages.
