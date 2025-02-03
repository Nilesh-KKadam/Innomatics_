<!-- Personal Budget Tracker By nilesh Kadam -->
<!DOCTYPE html>
<html lang="en">
<!-- Header Section start -->
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Budget Tracker</title>
</head>

<body style="background-color: #f0f4f7; margin: 0; padding: 0; color: #333;">
    <header style="background-color: #130436; color: white; padding: 20px 0; text-align: center;">
        


        <h1 style="font-size: 2.5rem; margin: 0;">Personal Budget Tracker 💸</h1>
        <nav style="margin-top: 100px;">
            <a href="#add-expense" style="color: #ffcc00; font-weight: bold; margin-right: 15px; text-decoration: none; font-size: 1.1rem;">Add Expenses 🛒 ➕ 🏠</a> |
            <a href="#view-budget" style="color: #ffcc00; font-weight: bold; margin-left: 10px; text-decoration: none; font-size: 1.1rem;">know yourBudget 💳</a>
        </nav>
    </header>

           <!-- Header Section End -->

           
           
           <!-- Section start -->

    <section id="add-expenses" style="padding: 30px 15%; background-color: rgb(255, 255, 255); border-radius: 10px; margin-top: 30px; box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);">
        <h2 style="text-align: center; color: #2d3e50;">Add Income/Expenses</h2>
        <form id="budget-form" style="display: flex; flex-wrap: wrap; justify-content: space-between; gap: 20px;">
            <div style="flex: 1; min-width: 250px;">
                <label for="income" style="display: block; margin-bottom: 5px; font-weight: bold;">Income 💵:</label>
                <input type="number" id="income" name="income" required style="width: 100%; padding: 10px; border-radius: 8px; border: 1px solid #ccc;">
            </div>
            <br>

            <div style="flex: 1; min-width: 250px;">
                <label for="expense" style="display: block; margin-bottom: 5px; font-weight: bold;">Expenses 💸:</label>
                <input type="number" id="expense" name="expense" required style="width: 100%; padding: 10px; border-radius: 8px; border: 1px solid #ccc;">
            </div>
            <br>
            <div style="flex: 1; min-width: 250px;">
                <label for="category" style="display: block; margin-bottom: 5px; font-weight: bold;">Category 📂:</label>
                <select id="category" name="category" required style="width: 100%; padding: 10px; border-radius: 8px; border: 1px solid #ccc;">
                    <option value="housing">🏠 Housing</option>
                    <option value="gym-membership">💪 Gym Membership</option>
                    <option value="furniture">🛋️ Furniture</option>
                    <option value="entertainment">🎮 Entertainment</option>
                    <option value="travel">✈️ Travel</option>
                    <option value="transportation">🚗 Transportation</option>
                    <option value="groceries">🥕 Groceries</option>
                    <option value="healthcare">💉 Healthcare</option>
                    <option value="insurance">🛡️ Insurance</option>
                    <option value="education">🎓 Education</option>
                    <option value="savings">💰 Savings</option>
                    <option value="dining-out">🍽️ Dining Out</option>
                    <option value="shopping">🛍️ Shopping</option>
                    <option value="utilities">💡 Utilities</option>
                    <option value="subscriptions">📅 Subscriptions</option>
                    <option value="miscellaneous">🔄 Miscellaneous</option>
                    <option value="phone-bill">📱 Phone Bill</option>
                </select>
            </div>

            <div style="flex: 1; min-width: 250px;">
                <label for="description" style="display: block; margin-bottom: 5px; font-weight: bold;">Add Note ✍️:</label>
                <input type="text" id="description" name="description" style="width: 100%; padding: 10px; border-radius: 8px; border: 1px solid #ccc;">
            </div>
            <br>

            <div style="flex: 1; min-width: 250px;">
                <label for="date" style="display: block; margin-bottom: 5px; font-weight: bold;">Select the Date 📅:</label>
                <input type="date" id="date" name="date" required style="width: 100%; padding: 10px; border-radius: 8px; border: 1px solid #ccc;">
            </div>

            <button type="submit" style="width: 100%; padding: 15px; background-color: #ffcc00; color: white; border: none; border-radius: 8px; cursor: pointer; font-size: 1.1rem; margin-top: 20px;">
                Submit ✅
            </button>
        </form>

        <div style="text-align: center; margin-top: 30px;">
            <label for="remaining" style="font-weight: bold;">Calculated Amount:</label>
            <input type="number" id="remaining" name="remaining" style="padding: 10px; width: 60%; font-size: 1.2rem; text-align: center; border: 2px solid #ffcc00; border-radius: 8px; background-color: #f9f9f9;">
        </div>

        <!-- Expenses Table -->
        <h3 style="text-align: center; margin-top: 40px;">Expenses List</h3>
        <table id="expenses-table" style="width: 100%; margin-top: 20px; border-collapse: collapse; text-align: left;">
            <thead>
                <tr style="background-color: #f3f3f3;">
                    <th style="padding: 10px; border: 1px solid #ccc;">Date</th>
                    <th style="padding: 10px; border: 1px solid #ccc;">Category</th>
                    <th style="padding: 10px; border: 1px solid #ccc;">Description</th>
                    <th style="padding: 10px; border: 1px solid #ccc;">Amount</th>
                    <th style="padding: 10px; border: 1px solid #ccc;">Actions</th>
                </tr>
            </thead>
            <tbody id="expense-list">
                <!-- Expense rows will be added here -->
            </tbody>
        </table>

        <textarea name="feedback" id="feedback" placeholder="Add your feedback here..." style="width: 100%; margin-top: 20px; padding: 15px; border-radius: 8px; border: 1px solid #ccc; font-size: 1rem;"></textarea>
        
        <button type="submit" style="width:; padding: 10px; background-color: #1e3bf7; color: white; border: none; border-radius: 20px; cursor: pointer; font-size: 1rem; margin-top: 20px;">
            Submit the Feedback
    </section>

    <!-- Section End -->


    <!-- Footer start -->

    <footer style="background-color: #2d3e50; color: white; padding: 30px 0; text-align: center; font-size: 16px; margin-top: 50px;">
        <div style="width: 70%; margin: 0 auto;">
            <p style="font-weight: 400;">© 2025 Personal Budget Tracker. All Rights Reserved by nilesh.k.kadam.</p>
            <p>
                <a href="#" style="color: #ffcc00; font-weight: 500; padding: 0 10px;">Terms & Conditions are apply.</a>
                
            </p>
            <p style="font-size: 14px;">By using this website, you agree to our <a href="#" style="color: #ffcc00;">Terms of Service</a> and <a href="#" style="color: #ffcc00">Privacy Policy</a>.</p>
        </div>
    </footer>
     <!-- Footer End -->

</body>

</html>


