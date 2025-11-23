Self Service Order Machine (Vue 3)
This is a small, simple self-service order machine interface built using HTML, CSS, and Vue 3. It allows users to select products, adjust quantities, and see a running total of their order summary.

🌟 Features
Product Selection: Click on an item to add it to your order.

Quantity Adjustment: Use the + and - buttons to change the quantity of a selected item.

Order Summary: A dynamic table shows the selected items, their quantities, and the running subtotal for each item.

Grand Total: The summary section automatically calculates and displays the final total amount.

Responsive Design: Uses basic CSS for a clean, two-column layout that should adapt to different screen sizes.

🛠️ Technologies Used
HTML5

CSS3 (style.css)

JavaScript (scripts.js)

Vue.js 3 (Used via CDN for reactivity and component structure)

📂 Project Structure
index.html: The main HTML file containing the structure and Vue directives.

style.css: The CSS file for styling the application.

scripts.js: The JavaScript file containing the product data, the Vue application instance, and the total calculation logic.

img/: (Implied) Directory for product images (e.g., img/big-mac.png).

⚙️ How to Run
Save the files: Ensure index.html, style.css, and scripts.js are in the same directory.

Open in Browser: Double-click index.html to open it in your web browser.

Note: This is a front-end only application and does not connect to a back-end database.

💻 Code Highlights
index.html (Vue Directives)
Uses v-for to loop through the products array.

Uses @click to toggle the product.active state.

Uses :class="{ selected : product.active }" for dynamic styling when a product is selected.

Uses v-if="product.active" to show the quantity controls and to display selected items in the summary.

Uses @click.stop on quantity buttons to prevent the click event from propagating up to the parent product-selection area.

The final total is displayed using the total() method.