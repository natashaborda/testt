// Named Function //

function storeUsername(username) {
	sessionStorage.setItem('username', username);

	console.log(username); // Works - local scope
}

function getUsername(username) {
	return sessionStorage.getItem('username');
}

const myUsername = 'natashaborda';

storeUsername(myUsername);

getUsername();

// //

const person = {
	firstName: 'Natasha',
	lastName: 'Borda',
	city: 'Union City',
	state: 'NJ',
	country: 'United States',
	age: 24,
	gender: 'female'
	getAddress: function() {
		return this.city + ', ' + this.state + ', ' + this.country; 
	}
};

// Local scope approach //
function getFullName(firstName, lastName) {
	return firstName + ' ' + lastName;
}

function getAddress(city, state, country) {
	return city + ', ' + state + ', ' + country;
}

function getAge(age) {
	return age;
}

function getGender(gender) {
	return gender;
};

getFullName(person.firstName, person.lastName);
getAddress(person.city, person.state, person.country);
getAge(person.age);
getGender(person.gender);

// Method Approach //

person.getAddress();


const name = 'Natasha Borda';

name.toLowerCase(); // 'natashaborda'

// Example 2 //
const pet = {
	firstName: 'Luna',
	species: 'Cat',
	age: 2,
	furColor: 'grey',
	birthMonth: 'May',
	city: 'Aeshboro',
	state: 'North Carolina'
	country: 'United States',
	gender: 'female'
};

// Local scope approach //
function getFullName(firstName) {
	return firstName;
}

function getAddress(city, state, country) {
	return city + ', ' + state + ', ' + country;
}

function getAge(age) {
	return age;
}

function getGender(gender) {
	return gender;
}

function getSpecies(species) {
	return species;
}

function getFurColor(furColor) {
	return furColor;
}

function getBirthMonth(birthMonth) {
	return birthMonth;
};

getFullName(pet.firstName);
getAddress(pet.city, person.state, person.country);
getAge(pet.age);
getGender(pet.gender);
getSpecies(pet.species);
getFurColor(pet.furColor);
getBirthMonth(pet.BirthMonth);


// In Class Practice //

let x = 6;
let y = 15;


function add(x,y) {
	return x + y; 
}

function subtract(x,y) {
	return x - y;
}

function multiply(x,y) {
	return x * y;
}

function division(x,y) {
	return x/y;
}

add(x,y)
