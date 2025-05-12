# Community Box Fire - Professional Directory

A community-driven professional directory for sharing and discovering services offered by gym community members. The interface is in Spanish while maintaining English-based project structure.

## 🚀 Features

- Tag-based filtering
- Full-text search
- Professional profiles with:
  - Name
  - Tags/Skills
  - Description
  - Contact information (phone, WhatsApp, email, Telegram)
  - Optional profile image

## 📋 Project Structure

```
community-box-fire/
├── content/
│   └── professionals/     # Professional listings (Spanish content)
├── static/
│   └── images/           # Profile images
└── layouts/              # Templates and search
```

## 🛠️ Setup Instructions

1. Install Hugo:
   ```bash
   # macOS (using Homebrew)
   brew install hugo

   # Windows (using Chocolatey)
   choco install hugo -confirm
   ```

2. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/community-box-fire.git
   cd community-box-fire
   ```

3. Start the development server:
   ```bash
   hugo server -D
   ```

4. View the site at: http://localhost:1313

## 📝 Adding a New Professional

1. Create a new markdown file in `content/professionals/`
2. Use this template:
   ```yaml
   ---
   title: "Full Name"
   date: YYYY-MM-DD
   tags: ["tag1", "tag2"]
   contact:
       phone: "+34 XXX XXX XXX"
       whatsapp: "+34 XXX XXX XXX"
       email: "email@example.com"
       telegram: "@username"
   image: "/images/professionals/filename.jpg"  # Optional
   draft: false
   ---
   Your description in Spanish...
   ```

### Draft vs Published
- `draft: true` - Content only visible when running locally with `hugo server -D`
- `draft: false` - Content visible both locally and on the live site

Use drafts while preparing content, then set to `false` when ready to publish.

3. (Optional) Add profile image to `static/images/professionals/`

## 🔍 Search and Filtering

- Use tags to categorize professionals
- Full-text search across all fields
- Filter by multiple tags

## 🚀 Deployment

This site is deployed using GitHub Pages. To deploy:

1. Push changes to the `main` branch
2. GitHub Actions will automatically build and deploy the site

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/NewFeature`)
3. Commit your changes (`git commit -m 'Add NewFeature'`)
4. Push to the branch (`git push origin feature/NewFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.