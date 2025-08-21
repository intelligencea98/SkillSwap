# Supabase Database Setup Instructions

The database schema needs to be set up in your Supabase project. Follow these steps:

## Option 1: Using Supabase Dashboard (Recommended)

1. Go to your Supabase project dashboard
2. Navigate to the **SQL Editor** tab
3. Copy the entire contents of `supabase/migrations/complete_schema_setup.sql`
4. Paste it into the SQL Editor
5. Click **Run** to execute the script

## Option 2: Using Supabase CLI (if available)

If you have the Supabase CLI installed and configured:

```bash
supabase db push
```

## What This Sets Up

The migration will create:

- **users table**: User profiles and authentication data
- **tasks table**: Task postings and management
- **task_applications table**: Applications to tasks  
- **contact_requests table**: Contact information sharing requests
- **Proper foreign key relationships** between all tables
- **Row Level Security (RLS)** policies for data protection
- **Indexes** for better query performance
- **Sample data** for testing

## After Setup

1. Restart your development server
2. The application should now work with the database
3. You can test with the demo account: `demo@skillswap.com` / `demo123`

## Troubleshooting

If you encounter any issues:

1. Check that your `.env` file has the correct Supabase credentials
2. Verify the migration ran successfully in the Supabase dashboard
3. Check the browser console for any remaining errors
4. Use the Supabase Diagnostic page in the app to verify the setup