# <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Food Share - Donate Leftover Food</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 50px; background-color: #f4f4f4; }
        .container { background: white; padding: 20px; border-radius: 8px; box-shadow: 0px 0px 10px #ccc; max-width: 400px; }
        input, select, button { width: 100%; padding: 10px; margin: 10px 0; border: 1px solid #ddd; border-radius: 4px; }
        button { background-color: #28a745; color: white; border: none; font-size: 16px; cursor: pointer; }
    </style>
</head>
<body>
    <div class="container">
        <h2>Donate Leftover Food</h2>
        <form action="/donate" method="POST">
            <input type="text" name="food_item" placeholder="Food Item Name (e.g., Rice, Biryani)" required>
            <input type="number" name="quantity" placeholder="Quantity (No. of Plates)" required>
            <input type="text" name="location" placeholder="Pickup Location Address" required>
            <select name="expiry_time">
                <option value="2 hours">Expires in 2 Hours</option>
                <option value="6 hours">Expires in 6 Hours</option>
                <option value="12 hours">Expires in 12 Hours</option>
            </select>
            <button type="submit">Submit Food Donation</button>
        </form>
    </div>
</body>
</html>index.html
