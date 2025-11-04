// Random Number Generator & Color Picker
function generateRandom(min, max) {
    return Math.floor(Math.random() * (max - min + 1)) + min;
}

const colors = ['red', 'blue', 'green', 'yellow', 'purple'];
const randomColor = colors[generateRandom(0, colors.length - 1)];

console.log(`Random number: ${generateRandom(1, 100)}`);
console.log(`Random color: ${randomColor}`);

const matrix = Array(3).fill(0).map(() => 
    Array(3).fill(0).map(() => generateRandom(1, 9))
);

console.log('Random matrix:', matrix);
