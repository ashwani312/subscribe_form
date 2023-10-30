## Subscription Management App

This is a Proof of Concept (POC) app demonstrating a subscription-based billing module using Next.js, Tailwind CSS, Node.js, and Stripe. Users can register, log in, choose a subscription plan, provide payment information, manage subscriptions, and view plan details.

### Features:
1. **User Registration and Login:**
   - Users can register for a new account.
   - Existing users can log in using their credentials.

2. **Available Plans:**
   - Plans and their details are fetched from the database and displayed to the users.

3. **Subscription Selection:**
   - Users can select a plan and choose the billing interval (monthly/yearly).

4. **Payment Information:**
   - Users can provide credit card information (using test cards) after selecting a plan.

5. **Subscription Creation:**
   - Utilizes Stripe APIs to create a recurring subscription for the user on the Stripe platform.
   - Subscription details are stored both in your database and Stripe.

6. **Subscription Management:**
   - Users can view their selected plan details.
   - Provides an option to cancel the selected plan.

### Test Cases Covered:
1. Users can create a new account.
2. Users can log in to existing accounts.
3. Initially, there are no subscriptions.
4. Users can create a subscription.
5. Users can cancel their subscription.

### Technologies Used:
- **Frontend:** Next.js, Tailwind CSS
- **Backend:** Node.js
- **Database:** (Not specified in the requirements, can use any database like MongoDB, MySQL, etc.)
- **Payment Gateway:** Stripe

### Running the App:
1. Clone the repository: `git clone https://github.com/ashwani312/subscribe_form.git`
2. Navigate to the project directory: `cd subscription-management-app`
3. Install dependencies: `npm install`
4. Set up environment variables:
   - Create a `.env.local` file with the following variables:
     ```
     STRIPE_PUBLIC_KEY=your_stripe_public_key
     STRIPE_SECRET_KEY=your_stripe_secret_key
     DB_CONNECTION_STRING=your_database_connection_string
     ```
5. Run the app: `npm run dev`

### How to Use:
1. Visit the app and register for a new account or log in with existing credentials.
2. Browse available plans, select a plan, and choose the billing interval.
3. Provide payment information using the test card details.
4. After successful payment, the selected plan details will be displayed.
5. Users can cancel their subscription at any time.

### Video Demo:
[Provide the link to your video demo here.]

### Future Improvements:
- Implement email notifications for successful subscription and cancellation.
- Add a feature for updating billing information.
- Enhance the UI/UX for a more user-friendly experience.

### Note:
- This app is a proof of concept and might require additional features and security measures for a production-ready application.
- Ensure proper error handling and security practices before deploying to a live environment.
