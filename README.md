# BCG Treatment Schedule Generator

A web application for generating and managing BCG treatment schedules following the SWOG protocol for bladder cancer patients.

## Features

- Generate complete treatment schedules based on TURBT date
- Visual timeline display
- Detailed clinical schedule with date ranges
- Copyable format for medical notes
- Mobile-responsive design

## Getting Started

### Prerequisites

- Node.js 16.x or higher
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/matt32l/bcg-scheduler.git
cd bcg-scheduler
```

2. Install dependencies:
```bash
npm install
```

3. Run the development server:
```bash
npm run dev
```

Visit `http://localhost:3000` to view the application.

## Deployment

### Deploying to Vercel (Recommended)

1. Create a Vercel account at [vercel.com](https://vercel.com)
2. Install Vercel CLI:
```bash
npm i -g vercel
```

3. Deploy:
```bash
vercel
```

### Custom Domain Setup

1. In Vercel dashboard, go to your project
2. Navigate to "Settings" → "Domains"
3. Add your domain
4. Follow DNS configuration instructions

### Environment Variables

No environment variables are required for basic functionality.

## Clinical Documentation

This application follows the SWOG protocol as detailed in:
> Lamm DL, et al. Maintenance bacillus Calmette-Guerin immunotherapy for recurrent TA, T1 and carcinoma in situ transitional cell carcinoma of the bladder: a randomized Southwest Oncology Group Study. J Urol 2000;163:1124-1129.

## Suggested Additional Features

1. Patient Data Management:
   - Save/load patient schedules
   - Export to PDF
   - Email functionality

2. Calendar Integration:
   - Add to Google Calendar
   - iCal export
   - Outlook integration

3. Clinical Enhancements:
   - Side effect tracking
   - Dose modification calculator
   - Treatment compliance tracking

4. Provider Features:
   - Multi-patient dashboard
   - Treatment completion statistics
   - Protocol deviation alerts

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Authors

- M Lierz
- T Goodstein
- V Wong

## License

This project is licensed under the MIT License - see the LICENSE.md file for details

## Acknowledgments

- SWOG protocol authors
- Bladder Cancer Advocacy Network (BCAN)
- AUA/SUO guidelines committee