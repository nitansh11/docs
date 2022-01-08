 # Launch Form question format
 
{   
 &nbsp; &nbsp; &nbsp; &nbsp;name: string;
 &nbsp; &nbsp; &nbsp; &nbsp;type: string;
 &nbsp; &nbsp; &nbsp; &nbsp;title: string;
 &nbsp; &nbsp; &nbsp; &nbsp;footerText?: string;
 &nbsp; &nbsp; &nbsp; &nbsp;isCompulsary?: boolean;
 &nbsp; &nbsp; &nbsp; &nbsp;placeholder?: string;
 &nbsp; &nbsp; &nbsp; &nbsp;radioOptions?: {
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;key: string;
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;value: string;
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;subtext?: string;
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;customSize?: string;
 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;}[];
 &nbsp; &nbsp; &nbsp; &nbsp;dropdownOptions?: string[];
}

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