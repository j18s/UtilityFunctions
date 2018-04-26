# UtilityFunctions
```
function toTitleCaseExcludingAbbreviation(data){
    function isUpperCase(str) {
        return str === str.toUpperCase();
    }
    const ary = data.trim().split(' ');
    
    let output = [];
    ary.map((element) => {
        if (isUpperCase(element)) {
            output.push (element);
        }
        else {
            output.push(element.toLowerCase());
        }
    });
    let finalString = output.join(' ');
    return finalString.replace(finalString.charAt(0), finalString[0].toUpperCase());
}

```
