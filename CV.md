1. Raxmonberdiyev Abduxalil Shavkat o‘g‘li
2. Phone number : +998 90 101 21 33
3. I'm junior FrontEnd developer . I want to upgrade my skills, knowladges, practice experience and et.c. Now a days I work in "TIIAME"MTU as engineer-programmer. This is my position. Actually, I didn't, doesn't, will not do anything about my direction . Why? Because universitys stuffs separate incorrect position and didn't support stuffs idea and requirements. What chief say do anything without any ignore. For example my side , my daily work is prepare pc such as fixing internet problem, lining up ethernet cables, transit any notifications and each small technical work. This is easy work from one side, but other side this works is ineffective and vain. That's why , I must upgrade programming skills and work as I want. These targets have in each person . And I do anything for my dreams and targets, if this being without results too. Go ahead ! ! !
4.  C++(basic) ,HTML, CSS, Bootstrap, JS, ReactJS, Redux (basic), Python(basic), Matlab(Simulink model basic), MissionPlanner(working with APM2.X FC), Photoshop and MasterSCADA(basic).
5. Task from Codewars (Link to task : https://codewars.com/kata/566584e3309db1b17d000027/train/javascript)
*** Differentiate a polynomial ****
// Instruction \\
Create a function that differentiates apolynomial for a given value of x.
Your function will receive 2 arguments: a polynomial as string and a point to evaluate the equation as an integer.

Assumptions:
* There will be a coefficient near each x,
unless the coefficient equals 1 or -1.
* There will be an exponent near each x, unless the exponent equals 0 or 1.
* All exponents will be greater or equal to zero.

Examples:
differenatiate("12x+2", 3) ===> return 12
differenatiate("x^2+3x+2", 3) ===> returns 9

======= Solution =========

In 1 - argument taken polynomial written as a string (like "x^2+3x+2").
Differentiate it (find its derivative).
Plug in number for x and return the result of derrivative at that number .

Example :
* Polynomial: x^2 +3x +2
* Derrivative 2x + 3
* At x = 3: 2*3 + 3 = 9
Answer = 9

Then we splitting the polynomial into parts . It uses a small pattern (called a regular expression)
to cut the string into terms like :
"x^2 + 3x + 2"-> ["x^2", "+3x", "+2]"
This makes it easy to handle each term separately.

Differentiating each term
It checks what type of term it is :
* ax^n (like 4x^3):derrivative = a*n*x^(n-1)
* ax (like 3x): derrivative = just a (because derrivative of x is 1)
* constant (like +5) : derrivative =0 (constants disappear)
It builds the new derrivative string term by term.

Code :
function differentiate(poly,xVal) {
    // Split polynomial into terms (keeping + or -)
    const terms = poly.match(/[+-]?\d*x\^\d+|[+-]?\d*x|[+-]?\d+/g);

    let derivativeTerms = [];

    for (let term of terms){
        if (term.includes('x^')){ // formax^n
            let [coeffStr, expStr] = term.split('x^');
            coeffStr = coeffStr.replace('+', '');
            let coeff = (coeffStr === '' ? 1 : (coeffStr === '-' ? -1 : parseInt(coeffStr)));
            let exp = parseInt(expStr);
            let newCoeff = coeff * exp;
            let newExp = exp - 1;

            if ( newExp === 0 ){
                dervativeTerms.push(`${newCoeff}`);
            } else if ( newExp === 1 ){
                derivativeTerms.push(`${newCoeff}x`);
            } else {
                derivativeTerms.push(`${newCoeff}x^${newExp}`);
            }

            else if (term.includes('x')) //form ax
            let coeffStr = term.replace('x',  '').replace('+', '');
            let coeff = (coeffStr === '' ? 1 : (coeffStr === '-' ? -1 : parseInt(coeffStr)));
            derivativeTerms.push(`${coeff}`);

         } else {
            // constant  -> derivative = 0 (ignore)
         }
    }

    // Join derivative string 
    let derivativeStr = derivativeTerms.join('+').replace(/\+\-/g, '-');
    if (derivative === '') return 0;

    // Evalute at xVal
    const evalStr = derivativeStr.replace(/x/g, `(${xVal})`);
    return eval(evalStr);
}

// Examples :
console.log(differentiate("12x+2",3))  //12
console.log(differentiate("x^2+3x+2", 3));  //9

2- Task (in  stage1/modules/algortihms/Readme.md)
Link for task : https://www.codewars.com/kata/fun-with-trees-array-to-tree https://www.codewars.com/kata/is-a-number-prime

Firstly we need given array of numbers, e.g. [17,0,-4,3,15]
We need to make a complete binary tree like this:
     17
    /   \
   0    -4 
  / \
 3   15 

The first item goes to the root.
Next two go to the root's children.
Next four go to the next level, and so on.
The node type is already defined:

var TreeNode = function(value, left, right){
    this.value = value;
    this.left = left;
    this.right = right;
};

function arrayTotree(array){
    if( !array || array.length === 0 ) return null;
    // Create nodes from array values
    let nodes = array.map(val => new TreeNode(val));

    // Link children 
    for (let i=0; i < nodes.length; i++){
        let leftIndex = 2 * i + 1;
        left rightIndex = 2 * i + 2;
        if ( leftIndex < nodes.length ){
            nodes[i].left = nodes[leftIndex];
        }
        if (rigthIndex < nodes.length){
            nodes[i].right = nodes[rightIndex];
        }
    }

    return  nodes[0]; // root node
}


6. See my work (inside of my resume) : https://www.secondresume.netlify.app

7. "TIIAME"MTU, Zako IT Academy, Shool21(Intensive), JavaScript Developement Track - Udacity("Onemillion uzbek coders" project . Supported by President of Republic of Uzbekistan Sh.Mirziyoyev ), CodeLiber (HTML Learn Pro and JavaScript Learn Pro), Sammi(sammi.ac platform), JavaScript Zero to Hero (Mohirdev platform: mohirdev.uz), "Kiberxavfsizlik kursi"(UZBANONS - Hekerlar uchun ahloqsiz Python), interesting book - DIGITAL SECURITY (CYBER TERROR AND CYBER SECURITY - Ananda Mitra, PH.D.) and other

8. My English Level is B2