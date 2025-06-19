Data Preparation and Cleaning

  The dataset was loaded, and null values were checked and confirmed to be absent.
  
  Descriptive statistics were reviewed to understand the spread of values for sleep hours, daily social media usage, addiction levels, and mental health scores.
  
  Data was segmented based on academic levels for more granular insights.

📈 Correlation Analysis

  Strong correlations were observed across various metrics:

    Daily Usage vs. Mental Health:
    
    High School: -0.84
    
    Undergraduate: -0.81
    
    Graduate: -0.78

  Daily Usage vs. Sleep Hours:

    High School: -0.92
    
    Undergraduate: -0.84
    
    Graduate: -0.73

  Sleep Hours vs. Mental Health:

    High School: +0.90
    
    Undergraduate: +0.74
    
    Graduate: +0.62

These results show that increased time on social media is strongly associated with lower sleep and mental well-being.

🔍 Hypothesis Testing

  Three hypothesis tests were conducted to compare addiction scores:
    
  Graduate vs. Undergraduate – Undergraduates were more addicted (p < 0.05).
    
  High School vs. Graduate – High school students were significantly more addicted (p << 0.05).
    
  High School vs. Undergraduate – High schoolers again showed higher addiction levels.
    
  These tests support the hypothesis that younger students are more vulnerable to addiction.

🤖 Modeling

  Initially, KMeans clustering was attempted to segment users, but it didn’t capture inverse relationships well.
  To overcome this:

    A manual classification was built using Addiction Score and Sleep Hours.
    
    A Decision Tree model was trained using features like mental health, usage, and relationship conflict.
    
    A Random Forest Classifier was used for final prediction due to higher accuracy and robustness.
    
    The final model achieved:
    
    High accuracy in classifying addiction levels.
    
    Clear feature importance showing which variables impacted addiction most.

🌍 Demographic & Platform Insights

  Most Addictive Platforms: WhatsApp, TikTok, Instagram.
  
  Age 18–20: Highest addiction and lowest sleep.

Gender-Based Trends:

  Males: More likely to use YouTube, Facebook.
  
  Females: More active on TikTok, Instagram.
  
  Country Trends: Some countries showed high addiction scores and sleep loss.

📊 Dashboard

  An interactive Tableau dashboard was built with filters for:

    Country
    
    Age Group
    
    Gender

  Countries with both genders present

    Key visualizations include:
    
    KPIs (Addiction, Sleep, Mental Health)
    
    Country-wise map
    
    Age trend line charts
    
    Platform usage bar chart
    
    Gender breakdown pie chart


📝 Final Takeaways

    High social media use correlates with worse mental health and reduced sleep, especially in students aged 18–20.
    
    Females tend to use more socially engaging platforms, while males prefer content-heavy platforms.
    
    Predictive modeling can accurately classify high-risk users.
    
    The dashboard enhances understanding and allows dynamic exploration by demographic group.

