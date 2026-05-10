# 🚀 SNTL 84 — Next.js SaaS Starter

> **Automate What's Costing You Money**  
> A production-ready SaaS foundation built with Next.js 14, Stripe, Prisma, and Auth.js.

---

## 📦 What This Is

This is a **private fork** of the popular [next-saas-stripe-starter](https://github.com/mickasmt/next-saas-stripe-starter) by @mickasmt, customized for rapid deployment by **SNTL 84** (Milan · Surat, India).

Use this as your launchpad for subscription-based products, SaaS tools, and revenue-generating web applications.

---

## ⚡ Quick Start

### 1. Clone & Install

```bash
git clone https://github.com/SNTL84/sntl84-next-saas-stripe-starter.git
cd sntl84-next-saas-stripe-starter
pnpm install
```

### 2. Environment Setup

```bash
cp .env.example .env.local
```

Configure your environment variables:

| Variable | Description |
|----------|-------------|
| `NEXTAUTH_URL` | Your app URL (http://localhost:3000 for dev) |
| `NEXTAUTH_SECRET` | Random secret for JWT encryption |
| `DATABASE_URL` | Neon/PostgreSQL connection string |
| `STRIPE_SECRET_KEY` | Your Stripe secret key |
| `STRIPE_WEBHOOK_SECRET` | Stripe webhook endpoint secret |
| `RESEND_API_KEY` | Resend email API key |

##3 3. Database Setup

```bash
npx prisma db push
```

### 4. Run Development

```bash
pnpm dev
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **Next.js 14** | React framework with App Router |
| **TypeScript** | Type-safe development |
| **Auth.js v5** | Authentication (Google, GitHub, Email) |
| **Prisma** | Database ORM |
| **Neon** | Serverless PostgreSQL |
| **Stripe** | Payments & subscriptions |
| **Resend** | Transactional emails |
| **React Email** | Email templates |
| **Shadcn/ui** | UI component library |
| **Tailwind CSS** | Utility-first styling |

---

## 🎯 Features Included

- ✅ **Authentication** — OAuth (Google, GitHub) + Email magic links
- ✅ **Role-based Access** — User & Admin roles
- ✅ **Subscription Management** — Stripe Checkout + Customer Portal
- ✅ **Admin Dashboard** — Manage users, subscriptions, content
- ✅ **Email System** — Welcome emails, notifications
- ✅ **Dark Mode** — Toggle between light/dark themes
- ✅ **Type-safe** — Full TypeScript coverage
- ✅ **Server Actions** — Next.js 14 app router native

---

## 🚀 Deployment

### Vercel (Recommended)

1. Push to GitHub
2. Import project on [Vercel](https://vercel.com)
3. Add environment variables
4. Deploy

```bash
vercel --prod
```

---

## 🏗️ Project Structure

```
├── app/                 # Next.js App Router
│   ├── (auth)/         # Authentication routes
│   ├── (dashboard)/    # Protected user dashboard
│   ├── (marketing)/    # Landing pages
│   └── api/            # API routes & webhooks
├── components/          # React components
├── lib/                # Utilities, auth, db
├── prisma/             # Database schema
├── emails/             # React Email templates
└── public/             # Static assets
```

---

## 🔐 Security Checklist

Before going live:

- [ ] Update `NEXTAUTH_SECRET` to a strong random string
- [ ] Configure Stripe webhook endpoints
- [ ] Set up production database
- [ ] Enable Stripe test mode first
- [ ] Verify email sending works (Resend)
- [ ] Review CORS settings
- [ ] Add rate limiting

---

## 📝 Customization

### Branding

Update these files with your brand:

- `app/layout.tsx` — Metadata, title, description
- `app/(marketing)/page.tsx` — Landing page content
- `components/brand-logo.tsx` — Logo component
- `lib/config/site.ts` — Site configuration
- `emails/` — Email templates

### Pricing

Edit subscription plans in:

- `lib/config/subscriptions.ts` — Plan definitions
- Stripe Dashboard — Plan & price management

---

## 📚 Documentation

- [Next.js Docs](https://nextjs.org/docs)
- [Auth.js Docs](https://authjs.dev/)
- [Prisma Docs](https://www.prisma.io/docs)
- [Stripe Docs](https://stripe.com/docs)
- [Shadcn/ui Docs](https://ui.shadcn.com/)

---

## 🤝 Credits

Original starter by [@mickasmt](https://github.com/mickasmt/next-saas-stripe-starter).

Modified and maintained by **SNTL 84** — Milan, AI Workflow Developer, Surat, India.

---

## 📞 Contact & Support

| Platform | Link |
|----------|------|
| 🌐 Website | [desidevloper.com](https://desidevloper.com) |
| 💬 WhatsApp | [+91 97274 13309](https://wa.me/919727413309) |
| 💼 LinkedIn | [linkedin.com/in/sntl2784](https://linkedin.com/in/sntl2784) |
| 🐙 GitHub | [github.com/SNTL84](https://github.com/SNTL84) |

---

> **I Automate What's Costing You Money.**  
> Let me help you ship faster. Reach out for custom SaaS development, AI integrations, and workflow automation.

---

## 📄 License

MIT License — Fork of [mickasmt/next-saas-stripe-starter](https://github.com/mickasmt/next-saas-stripe-starter).
