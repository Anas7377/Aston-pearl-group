# Aston-pearl-group
Refund request form
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aston Pearl - Refund Request Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            background: white;
            border-radius: 8px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        h2 {
            text-align: center;
            color: #2C3E50;
        }
        label {
            font-weight: bold;
        }
        input, select, textarea {
            width: 100%;
            padding: 8px;
            margin: 8px 0;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        button {
            background: #2C3E50;
            color: white;
            padding: 10px;
            border: none;
            width: 100%;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background: #1A252F;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Aston Pearl - Refund Request Form</h2>
        <form action="send_email.php" method="POST" enctype="multipart/form-data">
            <label>Date:</label>
            <input type="date" name="date" required>
            
            <label>Property Address:</label>
            <input type="text" name="property_address" required>
            
            <label>Name of Booking Holder:</label>
            <input type="text" name="booking_holder" required>
            
            <label>Move-in Date:</label>
            <input type="date" name="move_in_date" required>
            
            <label>Booking Provider (Council Name):</label>
            <input type="text" name="booking_provider" required>
            
            <label>Amount to be Refunded:</label>
            <input type="number" name="refund_amount" required>
            
            <label>Bank Details for Refund:</label>
            <input type="text" name="account_holder" placeholder="Account Holder Name" required>
            <input type="text" name="sort_code" placeholder="Sort Code" required>
            <input type="text" name="account_number" placeholder="Account Number" required>
            
            <label>Proof of Payment / Receipt:</label>
            <input type="file" name="proof_of_payment" required>
            
            <button type="submit">Submit Request</button>
        </form>
    </div>
</body>
</html>
