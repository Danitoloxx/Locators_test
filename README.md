# Locators Exercises

**The purpose of this exercise is to learn and practice about locators, different strategies and how
to name them properly.
For this practice, we will use this *[Website](https://www.demoqa.com/)* from which we will obtain the elements that need to be
defined. Each exercise will relate to a specific element in the page and the format in which the
element must be defined.**

## Exercises
1. In the landing *[page](https://www.demoqa.com/)*, define the card “Elements” using xpath -- > //div[@class='card mt-4 top-card'][1]

1. In this *[page](https://www.demoqa.com/text-box)*, define the following elements:
   * Full name: using css selector by Id -- > input[id='userName']
   * Email: css selector by placeholder -- > input[placeholder='name@example.com']
   * Current Address: xpath by Id -- > //textarea[@id='currentAddress']
   * Permanent address: xpath by class -- > (//textarea[@class='form-control'])[2]
   * Submit (button): xpath AND css by Id -- > //button[@class='btn btn-primary'] y por CSS: button[id='submit']

1. In this *[page](https://www.demoqa.com/links)*, define the following elements:
   * Home: xpath and css selector by Id -- > //div/p/a[@id='simpleLink'] y por CSS: a[id='simpleLink']
   * No Content: xpath by href -- > (//div/p/a[contains(@href,'javascript:void(0)')])[2]
   * List of links: xpath and css selector by tag (all the links) -- >  (//div/p/a)[depende del link coloco el numero para seleccionarlo] xpath y por CSS: p > a 

1. In this *[page](https://www.demoqa.com/accordian)*, define the following elements:
   - What is Lorem Ipsum? xpath and css selector by class -- > (//div[@class='card-header'])[1] y por CSS: div[class='card-header'][id='section1Heading'] 
   - Why do we use it? (To expand or collapse the text click on the link)
     - Text inside closed by xpath using the class attribute. -- > (//div[@class='collapse'])[3]
     - Text inside expanded by css selector using the class attribute. -- > #section3Content > p <- css selector (class is empty)

1. In this *[page](https://www.demoqa.com/date-picker)*, deﬁne the following elements:
   * Select date: xpath by value -- > //input[@value='07/20/2021']
   * Date and time: css selector by value. -- > input[value='July 20, 2021 2:31 PM']

## Extra Credits

This *[page](https://riptutorial.com/xpath/example/6209/find-all-elements-with-certain-text)* will be useful for the following exercises. However, feel free to search on the internet
anything that is not explained there.

1. In this *[page](https://www.demoqa.com/)*, obtain the text of the element called “Interactions” using xpath -- > string((//div/h5)[1])
1. In this *[page](https://www.demoqa.com/elements)*, obtain the text from the following elements:
   * Text Box -- > string(//span[contains(text(), 'Text Box')])
   * Buttons -- > string(//span[contains(text(), 'Buttons')])
   * Broken Links - Images -- > string(//span[contains(text(), 'Broken Links - Images')])
1. Create an xpath to match a span (located in the footer) that CONTAINS the text “QA" -- > //footer/span[contains(text(), 'QA')]
1. How would you change the xpath defined in the previous exercise to match ALL
ELEMENTS that CONTAIN the text QA. -- > //*span[contains(text(), 'QA')] (PREGUNTAR)



