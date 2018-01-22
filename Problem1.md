var fullname = 'John Doe';
var obj = {
   fullname: 'Colin Ihrig',
   prop: {
      fullname: 'Aurelio De Rosa',
      getFullname: function() {
         return this.fullname;
      }
   }
};

console.log(obj.prop.getFullname());

var test = obj.prop.getFullname;

console.log(test());


/*OUTPUT
"Aureli De Rosa"
"John Doe" */
/* In the first console.log() call, getFullname() is invoked as a function of the obj.prop object so, 
 the function returns the fullname property of this object. when getFullname() is assigned to the test
 variable, the context refers to the global object which was initialised at the beginning. 
 This happens because test is implicitly set as a property of the global object. */
