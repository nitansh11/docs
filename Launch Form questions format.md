 # Launch Form question format
 
{   
 &nbsp; &nbsp; &nbsp; &nbsp;name: string;<br />
 &nbsp; &nbsp; &nbsp; &nbsp;type: string;<br />
 &nbsp; &nbsp; &nbsp; &nbsp;title: string;<br />
 &nbsp; &nbsp; &nbsp; &nbsp;footerText?: string;<br />
 &nbsp; &nbsp; &nbsp; &nbsp;isCompulsary?: boolean;<br />
 &nbsp; &nbsp; &nbsp; &nbsp;placeholder?: string;<br />
 &nbsp; &nbsp; &nbsp; &nbsp;radioOptions?: {<br />
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;key: string;<br />
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;value: string;<br />
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;subtext?: string;<br />
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;customSize?: string;<br />
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;}[];<br />
 &nbsp; &nbsp; &nbsp; &nbsp;dropdownOptions?: string[];<br />
}<br />

## Uses:

Explanation:

*   **name**: this is a unique key for a question
*   **type**: it can be "input" or "dropdown" or "radio"
*   **title**: this is the question text
*   **footerText**: this is optional field, if we want to put a note below the question
*   **placeholder**: Required only if type is "input",
*   **radioOptions**: Required only if type is "radio", below are the value needed for a single radio value
*       key: should be unique text for each option
        value: text which will be shown to user for a option
	    subtext: subtext shown below option value to user
        customSize: "regular" or "large" of a radio button.
*   **dropdownOptions**: Required only if type is "dropdown", it will be a array/collection if values which we want to show to user.
