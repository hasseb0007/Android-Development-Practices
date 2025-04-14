### Key Points
- Research suggests that having two separate subscriptions (monthly and yearly) for the same features may confuse users and increase management complexity.
- It seems likely that consolidating into one subscription with multiple base plans (monthly and yearly) simplifies operations and improves user experience.
- The evidence leans toward aligning with Google Play's recommended model for better flexibility in promotions and cost efficiency.

### Current Setup Issues
Your current setup, with two separate subscriptions for monthly and yearly plans that offer identical features but differ in price, can lead to several challenges:
- **User Confusion**: Users might find it hard to switch between plans or accidentally purchase both, leading to redundant payments.
- **Management Complexity**: Managing two SKUs increases operational workload and potential errors in pricing and availability settings.
- **Limited Flexibility**: It's harder to offer promotions like discounts for upgrades or regional pricing with separate subscriptions.

### Recommended Approach
Switching to one subscription with two base plans (monthly and yearly) and adding offers for each plan is likely better:
- **Simplified Management**: All plans are under one subscription, reducing administrative overhead.
- **Improved User Experience**: Users can easily switch plans, and Google Play handles upgrades seamlessly.
- **Enhanced Flexibility**: You can attach offers like introductory pricing or upgrade discounts to each base plan, tailoring strategies to user segments.

### Supporting Evidence
Google Play's documentation, updated in May 2022, recommends this model for its flexibility and efficiency. For example, [Understanding subscriptions](https://support.google.com/googleplay/android-developer/answer/12154973?hl=en) explains how a single subscription can have multiple base plans, each with offers for discounts.

---

### Survey Note: Detailed Analysis of Subscription Structure for Android VPN App

This note provides a comprehensive analysis of the subscription structure for your Android VPN app on Google Play, focusing on the current setup (two separate subscriptions for monthly and yearly plans, identical in features but differing in price, presented as one subscription with two plans) and the proposed change to one subscription with two base plans and added offers. The analysis is grounded in official Google Play documentation and developer resources, ensuring a thorough understanding of best practices and potential issues.

#### Background and Context
Your app currently operates with two subscription flows: a monthly plan and a yearly plan, both offering the same features but at different price points. These are presented to users as one subscription with two plans. However, Google Play introduced significant changes to its subscription model in May 2022, shifting from a legacy system of multiple independent subscriptions to a more flexible model where a single subscription can have multiple base plans and offers. This shift aims to simplify management, enhance user experience, and reduce operational costs for developers.

#### Analysis of Current Setup
The current setup, with two separate subscriptions for monthly and yearly plans, aligns with the legacy system, which has several documented drawbacks:

1. **Complexity in Management**:
   - In the legacy system, subscriptions were defined as fully independent objects, each with a single billing period, price, and potential free trial or introductory pricing. This meant that for the same set of benefits (e.g., your VPN features), developers had to manage multiple SKUs, ensuring consistency in user-facing descriptions and benefits across subscriptions.
   - For your app, this translates to managing two separate SKUs (one for monthly, one for yearly), which increases operational complexity. Each SKU requires separate configuration in the Play Console, including pricing, availability by region, and promotional settings, leading to potential errors and higher administrative overhead.
   - Official documentation, such as [Recent changes to subscriptions in Play Console](https://support.google.com/googleplay/android-developer/answer/12124625?hl=en), highlights that this approach was common in the past but is now considered less efficient due to the need to prevent redundant purchases and ensure consistency.

2. **User Confusion and Redundant Purchases**:
   - Users may find it confusing to manage two separate subscriptions for what is essentially the same product with different billing periods. For instance, if a user starts with the monthly plan and later wants to switch to the yearly plan, they might not understand how to do so seamlessly, potentially leading to frustration.
   - There is also a risk of redundant purchases, where users might accidentally subscribe to both plans, thinking they are different products. This can result in customer support issues, refunds, and negative user feedback, impacting retention and satisfaction.
   - The documentation emphasizes that the new model simplifies user interaction by allowing seamless switching between base plans under a single subscription, reducing such confusion.

3. **Operational Costs and Inefficiencies**:
   - Managing multiple SKUs increases operational costs, as each subscription requires separate monitoring, analytics, and updates. For example, if you need to adjust pricing or add a promotional offer, you must do so for each SKU independently, doubling the effort.
   - The [Android Developers Blog: Purchase optimization, flexible subscriptions, and revenue growth with Play Commerce](https://android-developers.googleblog.com/2022/11/optimization-flexibility-and-growth-with-play-commerce.html) notes that the new model reduces the need for multiple SKUs, thereby lowering operational costs by consolidating management under a single subscription product.

4. **Limited Flexibility for Promotions**:
   - With two separate subscriptions, it is challenging to implement flexible promotional strategies, such as offering discounts for upgrading from monthly to yearly, introductory pricing for new subscribers, or region-specific pricing. Each subscription would need its own promotional settings, limiting your ability to tailor offers to user segments.
   - The new model allows for offers to be attached to each base plan, providing greater flexibility. For example, you could offer a 20% discount for users upgrading to the yearly plan or provide a free trial month for new subscribers, all managed under one subscription.

5. **Analytics and Reporting Challenges**:
   - Having two separate subscriptions complicates analytics and reporting, as metrics like churn rate, retention, and revenue are tracked separately for each SKU. This can make it harder to get a holistic view of subscription performance and identify trends.
   - Consolidating into one subscription with multiple base plans allows for better visibility into overall subscription metrics, as all plans are part of the same product, simplifying reporting and decision-making.

#### Recommended Approach: One Subscription with Multiple Base Plans and Offers
Given the issues with the current setup, switching to one subscription with two base plans (monthly and yearly) and adding offers for each plan is the recommended approach. This aligns with Google Play's best practices and offers several advantages:

1. **Simplified Management**:
   - Under the new model, you create a single subscription product that encompasses all features of your VPN app. Within this subscription, you define two base plans: one for monthly billing and one for yearly billing, each with its own price and renewal type (auto-renewing).
   - This consolidation reduces the number of SKUs to manage, streamlining configuration in the Play Console. For example, pricing updates, regional availability, and promotional settings can be managed centrally, reducing administrative effort.
   - [Understanding subscriptions](https://support.google.com/googleplay/android-developer/answer/12154973?hl=en) explains that a base plan defines the billing period, renewal type, and price, and a single subscription can have multiple base plans, making this approach feasible.

2. **Improved User Experience**:
   - Users benefit from a clearer understanding of subscription options, as all plans are presented under one product. They can easily switch between monthly and yearly billing periods without dealing with separate subscriptions, enhancing usability.
   - Google Play handles upgrades and downgrades seamlessly, ensuring a smooth experience. For example, if a user upgrades from monthly to yearly, the system can prorate charges and manage the transition, reducing user friction.
   - This aligns with the goal of improving retention, as noted in the [Android Developers Blog: New flexible tools to grow your subscription business](https://android-developers.googleblog.com/2022/05/new-ways-to-sell-subscriptions-on-google-play_0530335598.html), which emphasizes user-friendly subscription management.

3. **Enhanced Flexibility in Promotions**:
   - Each base plan can have multiple offers, such as introductory pricing, discounts for upgrades, or special promotions for specific regions or user segments. For example, you could offer a 50% discount for the first year for new subscribers on the yearly plan or a free month for users upgrading from monthly to yearly.
   - This flexibility allows you to tailor your pricing strategy to attract new users, retain existing ones, and recover at-risk subscribers, aligning with best practices outlined in [Sell subscriptions](https://developer.android.com/google/play/billing/subscriptions).

4. **Cost Efficiency**:
   - By reducing the number of SKUs, you lower operational costs associated with managing multiple subscriptions. This includes reduced effort in configuration, monitoring, and updates, as well as potentially lower fees for managing additional SKUs.
   - The blog post on [Purchase optimization, flexible subscriptions, and revenue growth with Play Commerce](https://android-developers.googleblog.com/2022/11/optimization-flexibility-and-growth-with-play-commerce.html) highlights that this model reduces operational costs by eliminating the need for an ever-increasing number of SKUs.

5. **Future-Proofing and Scalability**:
   - Aligning with Google Play's current model ensures your app can easily adopt future enhancements, such as prepaid plans, advanced analytics, or new promotional tools. This is particularly important as Google Play continues to evolve its subscription features, as noted in [May 2022 subscription changes guide](https://developer.android.com/google/play/billing/compatibility).

#### Implementation Details
To implement this change, follow these steps:
- **Create a Single Subscription**: In the Play Console, create a new subscription product that represents your VPN service, including all features.
- **Add Base Plans**: Under this subscription, create two base plans: one for monthly billing (e.g., $9.99/month, auto-renewing) and one for yearly billing (e.g., $99.99/year, auto-renewing). Configure pricing and availability for each.
- **Add Offers**: Attach offers to each base plan, such as:
  - An introductory offer for new subscribers (e.g., first month free for monthly plan, first year at 50% off for yearly plan).
  - An upgrade offer for users switching from monthly to yearly (e.g., 20% discount for the first year).
  - Regional promotions for specific countries (e.g., discounted pricing in emerging markets).
- **Update User Interface**: Ensure your app's UI reflects this structure, presenting the subscription as one product with monthly and yearly options, and clearly displaying any offers.

#### Potential Challenges and Mitigation
While transitioning to this model, you may face some challenges:
- **Migration Effort**: Updating existing subscriptions to the new model may require technical changes, especially if your backend relies on legacy APIs. Use the [May 2022 subscription changes guide](https://developer.android.com/google/play/billing/compatibility) for migration guidance, ensuring compatibility with Play Billing Library version 5 or newer.
- **User Communication**: Inform users about the change to avoid confusion. Use in-app notifications and emails to explain the new structure and highlight benefits like easier plan switching and promotional offers.
- **Analytics Adjustment**: Initially, you may need to adjust analytics to track metrics under the new structure. Use Google Play's subscription reporting tools ([Subscription reporting](https://play.google.com/console/about/subscriptionreporting/)) to monitor performance post-transition.

#### Conclusion
The evidence strongly supports switching to one subscription with multiple base plans and offers for your Android VPN app. This approach aligns with Google Play's best practices, simplifies management, improves user experience, and enhances flexibility for promotions, ultimately reducing operational costs and ensuring scalability. By addressing the complexities of the current setup, you can better serve your users and position your app for long-term success.

---

### Key Citations
- [Understanding subscriptions Play Console Help](https://support.google.com/googleplay/android-developer/answer/12154973?hl=en)
- [Recent changes to subscriptions in Play Console Help](https://support.google.com/googleplay/android-developer/answer/12124625?hl=en)
- [Purchase optimization flexible subscriptions revenue growth Android Developers Blog](https://android-developers.googleblog.com/2022/11/optimization-flexibility-and-growth-with-play-commerce.html)
- [Create and manage subscriptions Play Console Help](https://support.google.com/googleplay/android-developer/answer/140504?hl=en)
- [May 2022 subscription changes guide Google Play billing system Android Developers](https://developer.android.com/google/play/billing/compatibility)
- [Sell subscriptions Google Play billing system Android Developers](https://developer.android.com/google/play/billing/subscriptions)
- [New flexible tools to grow your subscription business Android Developers Blog](https://android-developers.googleblog.com/2022/05/new-ways-to-sell-subscriptions-on-google-play_0530335598.html)
- [Subscription reporting Google Play Console](https://play.google.com/console/about/subscriptionreporting/)
