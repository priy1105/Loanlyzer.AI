## 💰🚗 Loanlyzer.AI - AI-Powered Car Marketplace & Loan Evaluator 🚗💰
A comprehensive, full-stack vehicle marketplace that integrates cutting-edge AI for an intelligent car search experience and adds powerful financial tools for loan evaluation. Users can find their dream car using text or image-based searches, analyze their loan options with detailed amortization schedules, and export financial reports to PDF and CSV. The platform also includes a complete admin dashboard for managing inventory, test drives, and dealership settings.


## 🚀 Key Features
### User & Financial Features
AI-Powered Visual Search: Upload a car image and let Gemini AI find similar vehicles in the inventory.
Advanced Loan Evaluator: Generate detailed, month-by-month loan amortization schedules based on vehicle price, down payment, interest rate, and tenure.
PDF & CSV Export: Download and save your complete loan amortization schedule as a professional PDF or a data-rich CSV file for your financial records.
Advanced Filtering & Search: Filter cars by make, body type, fuel type, price range, and more to find the perfect vehicle.
Save Favorite Cars: Authenticated users can save cars to a personal wishlist for later viewing.
Real-Time Test Drive Booking: Schedule test drives using an interactive calendar that shows real-time availability based on dealership hours/_components/test-drive-form.jsx].

### Admin-Facing Features
Comprehensive Dashboard: Get a complete overview of the marketplace with statistics on cars, test drives, and conversion rates.
AI-Assisted Data Entry: Add new cars by uploading an image; Gemini AI automatically extracts and pre-fills the car's details, saving valuable time.
Full Inventory Management: Admins have complete CRUD (Create, Read, Update, Delete) control over the car listings.
Test Drive Management: View all test drive bookings, filter them, and update their status (e.g., Pending, Confirmed, Completed).
Settings Control: Manage dealership working hours and promote or demote user roles to control admin access.


## 🛠️ Tech Stack

Framework: Next.js 

Styling: Tailwind CSS & shadcn/ui

Database: PostgreSQL (via Supabase) 

ORM: Prisma

Authentication: Clerk

Artificial Intelligence: Google Gemini API  
Security & Rate Limiting: Arcjet    
File Storage: Supabase Storage    
Form Management: React Hook Form with Zod for validation     
PDF & CSV Generation: jsPDF, json2csv, charts.js, recharts    
UI Components: Radix UI     
Notifications: Sonner (for toasts)    

## 📦 Installation & Dependencies
To get this project running on your local machine, first clone the repository. Then, install all the necessary packages by running the command below in your project's root directory.

Bash
```
npm install
```
This will install all dependencies listed in the package.json file, including:
```
Core & Framework: next, react, react-dom
Styling & UI: tailwindcss, tailwindcss-animate, class-variance-authority, clsx, tailwind-merge, lucide-react, sonner, react-day-picker, and @radix-ui/* components.
Data & State Management: @prisma/client, @supabase/ssr, @supabase/supabase-js, react-hook-form, zod.
Authentication & Security: @clerk/nextjs, @arcjet/next.
AI & Utilities: @google/generative-ai, react-dropzone, date-fns, uuid.
Loan Schedule Exports: jspdf, jspdf-autotable, json2csv.
```







### Make sure to create a `.env` file with following variables -

```
DATABASE_URL=
DIRECT_URL=

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

GEMINI_API_KEY=

ARCJET_KEY=
```
