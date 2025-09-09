# React + Vite

# Install Vite 5 (latest minor in that line)
npm create vite@5 daily-expenses-tracker


daily-expenses-tracker/ 
│── public/                         # Static files (favicon, manifest, logos)
│
│── src/
│   │── api/                        # API integrations (localStorage / backend / Firebase)
│   │   └── expensesApi.js          # Functions to fetch/save expenses data
│   │
│   │── assets/                     # Images, fonts, icons
│   │
│   │── components/                 # Reusable UI components
│   │   ├── Navbar.jsx              # Top navigation bar (theme switcher, nav links)
│   │   ├── ExpenseForm.jsx         # Form to add/edit expenses
│   │   ├── ExpenseList.jsx         # List of all expenses
│   │   ├── ExpenseItem.jsx         # Single expense card/item
│   │   ├── SummaryCard.jsx         # Displays totals/summary
│   │   └── Chart.jsx               # Recharts/Chart.js component for visual reports
│   │
│   │── context/                    # Context API (if using Context instead of Redux)
│   │   ├── ExpenseContext.jsx      # Global state for expenses (useReducer + Context)
│   │   └── ThemeContext.jsx        # Global state for light/dark theme
│   │
│   │── features/                   # Redux slices (if using Redux Toolkit)
│   │   ├── expenses/
│   │   │   └── expensesSlice.js    # Redux slice for expenses (add/delete/update)
│   │   └── theme/
│   │       └── themeSlice.js       # Redux slice for theme (light/dark toggle)
│   │
│   │── hooks/                      # Custom React hooks
│   │   ├── useLocalStorage.js      # Persist state to localStorage
│   │   ├── useExpenses.js          # Hook wrapper for ExpenseContext or Redux selector
│   │   └── useTheme.js             # Hook wrapper for ThemeContext or Redux selector
│   │
│   │── pages/                      # Page-level views
│   │   ├── Home.jsx                # Dashboard (summary + list of expenses)
│   │   ├── AddExpense.jsx          # Page with ExpenseForm
│   │   ├── Reports.jsx             # Reports/analytics with charts
│   │   └── Settings.jsx            # User preferences (theme, reset data, etc.)
│   │
│   │── styles/                     # Styling
│   │   ├── globals.css             # Global TailwindCSS / base styles
│   │   └── themes.css              # Optional custom theme overrides
│   │
│   │── utils/                      # Helper functions
│   │   ├── formatDate.js           # Format date for display
│   │   ├── calculateTotals.js      # Calculate totals/summaries
│   │   └── categories.js           # List of default expense categories
│   │
│   │── App.jsx                     # Root component (wraps Router + Providers)
│   │── main.jsx                    # Entry point (ReactDOM.createRoot)
│   │── router.jsx                  # React Router config (routes for pages)
│   │── store.js                    # Redux store (only if Redux Toolkit is used)
│
│── package.json
│── vite.config.js
│── README.md
