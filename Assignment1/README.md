# Assigment 1


* *Date Created*: 01 FEB 2022
* *Last Modification Date*: 06 FEB 2022
* *Git URL*: <https://git.cs.dal.ca/vjoshi/csci5709.git>

## Authors

* [Viraj Joshi](viraj.joshi@dal.ca) 



### Prerequisites

To have a local copy of this assingnment up and running on your local machine, you will first need to install the following dependencies by running the following commands

```
Download all the packages and their dependencies - npm install
Run the web application - npm start

```

## Deployment

The developed feature is deployed on Netlify at URL - https://main--merry-sorbet-809a05.netlify.app/

## Built With

* [Reactjs](https://reactjs.org/) - The web framework used to build the web app.
* [CSS](https://www.w3.org/Style/CSS/Overview.en.html) - Styling the web app. 
* [Netlify](https://www.netlify.com/) - Used to deploy the application on web.
* [Visual Studio](https://code.visualstudio.com/) - Code editor. 


## Sources Used

### registration.js

*Lines 4 - 7*

```
const Modal = props => {
    if(!props.show){
        return null;
    }

```

The code above was created by adapting the code in [Medium.com](https://codesandbox.io/s/magical-christian-qxtdm?from-embed) as shown below: 

```
const Modal = props => {
  const closeOnEscapeKeyDown = e => {
    if ((e.charCode || e.keyCode) === 27) {
      props.onClose();
    }
  };

```

The code in [Medium.com](https://codesandbox.io/s/magical-christian-qxtdm?from-embed) was implemented to close the modal by an escape character. 
The code was referred to close the registration success modal on clicking the close button.
The Code was modified by changing the condition in if statement to check property ('props') value of 'show'. If show is false, modal would not be displayed.


### registration.js

*Lines 42 - 43*

```
const validEmail = new RegExp(
        '^[a-zA-Z0-9._:$!%-]+@[a-zA-Z0-9.-]+.[a-zA-Z]$'
    );

```

The code above was created by adapting the code in [w3resource](https://www.w3resource.com/javascript/form/email-validation.php) as shown below: 

```
function ValidateEmail(mail) 
{
 if (/^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/.test(myForm.emailAddr.value))
  {
    return (true)
  }
    alert("You have entered an invalid email address!")
    return (false)
}

```

The code in [w3resource](lihttps://www.w3resource.com/javascript/form/email-validation.phpnk) was implemented to validate an email using a regular expression.
The code was used to validate the entered email address.
The code was modified by setting the regular expression in a variable 'validEmail' and match it with the state value using the test function. 

## modal.CSS

*Lines 7 - 10 

```
    display: flex;
    justify-content: center;
    background-color: rgba(0, 0, 0, 0.5);

```
The code above was created by adapting the code in [Medium.com](https://codesandbox.io/s/magical-christian-qxtdm?from-embed) as shown below: 

```
.modal {
  position: fixed;
  left: 0;
  top: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  align-items: center;
  justify-content: center;
  opacity: 0;
  transition: all 0.3s ease-in-out;
  pointer-events: none;
}

```

The code in [Medium.com](https://codesandbox.io/s/magical-christian-qxtdm?from-embed) was implemented style the modal 
The code was referred to style the modal contents.
The code was modified by remove the css properties that were already known to me or were not needed for the purpose of simply displaying a success message. 

