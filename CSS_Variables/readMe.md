CSS Variables
also known as custom properties, are a native feature of the language implemented by most web browsers. They are useful for reducing repetition by the reuse of CSS code.

The second benefit of CSS variables is meaningful variable identifiers. For example, the variable name, --site-theme-color is a lot simpler to understand than say, #4a90e2(a shade of blue). This is particularly true in case this same color (#4a90e2) is used in various other contexts in a given application.

Syntax and basic usage
CSS variables are properties that begin with a double dash. For example, --site-theme-color is a valid CSS variable name

Scoping rules
Variables can be declared in global or local scope.

Declaring variables in the global scope
You can create globally scoped variables, which can be referenced by any CSS ruleset in the CSS document. They are declared under the :root pseudo class, like so:

:root {
--property-name: value
}
The :root pseudo class maps to the root element of the DOM tree (typically the <html> element).

Variable access
Variables can be accessed in two ways:

With the var() function
Variables are typically accessed with the var() function. The var() function is replaced with the value of the CSS variable.

With the calc() function
In most programming languages, we can assign an arithmetic expression to a variable. We can do this in CSS with the calc() function.

Cascade and Inheritance rules
Variables in CSS are subject to standard cascade and inheritance rules.

Fallback values
In a CSS statement (a property, value pair) with variables, if the variable name present in the statement is not yet defined, we can allow it to fall back to a default value with the help of the var() function.

The var() function supports a maximum of 2 arguments. The first argument is required to be present and denotes the name of the CSS variable to be replaced with a value. The second argument is optional, which if provided, becomes a fallback value if the first argument (the variable name) is not defined.
