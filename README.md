# feb-2025-avasjcript-events-and-basic-interactivity

Event Listeners: Use addEventListener to listen for specific events and trigger functions.

const button = document.getElementById('myButton');

button.addEventListener('click', function() {
  alert('Button clicked!');
});


Common Events: Examples include click, mouseover, keyup, submit, etc.

Event Object: Contains information about the event, such as the target element and mouse position.

<button id="myButton">Click Me</button>

<script>
  const button = document.getElementById('myButton');
  
  button.addEventListener('click', function() {
    alert('Button was clicked!');
  });
</script>


Form Events: Useful for handling form submission, validation, and changes.

<form id="myForm">
  <input type="text" id="name" name="name" required>
  <button type="submit">Submit</button>
</form>

<script>
  const form = document.getElementById('myForm');

  form.addEventListener('submit', function(event) {
    event.preventDefault(); // Prevent form from actually submitting
    alert('Form submitted!');
  });
</script>

Prevent Default: Use event.preventDefault() to prevent default browser behavior (e.g., form submission, link navigation).

<form id="myForm">
  <input type="text" id="name" name="name" required>
  <button type="submit">Submit</button>
</form>

<script>
  const form = document.getElementById('myForm');

  form.addEventListener('submit', function(event) {
    event.preventDefault(); // Prevent the form from submitting
    alert('Form submission blocked!');
  });
</script>

Event Propagation: Events bubble up or capture down the DOM tree. Use stopPropagation() to prevent bubbling.
