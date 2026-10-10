# MyCodingBot
My Repository



<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Gyanwali Ramesh is a Teacher, Trainer, and Digital Creator with 15+ years of experience in management, administration, teaching, and organizational development." />
  <title>Gyanwali Ramesh | Teacher, Trainer & Digital Creator</title>
  <style>
    :root {
      --navy: #0B1F3A;
      --royal: #2563EB;
      --white: #FFFFFF;
      --gray: #F3F6FA;
      --gold: #F4B942;
      --text: #1d2b3c;
      --muted: #5e6d85;
      --shadow: 0 18px 40px rgba(11, 31, 58, 0.12);
      --radius-lg: 24px;
      --radius-md: 16px;
      --radius-sm: 12px;
      --container: 1180px;
      --transition: 0.3s ease;
      --nav-height: 78px;
    }

    * { box-sizing: border-box; }

    html {
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: Inter, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
      color: var(--text);
      background: var(--white);
      line-height: 1.7;
      -webkit-font-smoothing: antialiased;
      text-rendering: optimizeLegibility;
    }

    img {
      max-width: 100%;
      display: block;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    button, input, textarea, select {
      font: inherit;
    }

    .container {
      width: min(var(--container), calc(100% - 32px));
      margin: 0 auto;
    }

    .section {
      padding: 96px 0;
    }

    .section-header {
      text-align: center;
      max-width: 760px;
      margin: 0 auto 44px;
    }

    .eyebrow {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: rgba(37, 99, 235, 0.08);
      color: var(--royal);
      border: 1px solid rgba(37, 99, 235, 0.12);
      border-radius: 999px;
      padding: 8px 16px;
      font-size: 0.82rem;
      font-weight: 700;
      letter-spacing: 0.08em;
      text-transform: uppercase;
    }

    .section-header h2 {
      font-size: clamp(2rem, 4vw, 3rem);
      line-height: 1.2;
      margin: 16px 0 12px;
      color: var(--navy);
    }

    .section-header p {
      margin: 0;
      font-size: 1.05rem;
      color: var(--muted);
    }

    /* Header / Nav */
    .site-header {
      position: sticky;
      top: 0;
      z-index: 1000;
      background: rgba(11, 31, 58, 0.88);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid rgba(255,255,255,0.08);
    }

    .nav-wrap {
      max-width: var(--container);
      width: min(var(--container), calc(100% - 24px));
      margin: 0 auto;
      min-height: var(--nav-height);
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 24px;
    }

    .brand {
      display: inline-flex;
      align-items: center;
      gap: 12px;
      font-weight: 800;
      letter-spacing: 0.02em;
      color: var(--white);
      white-space: nowrap;
    }

    .brand-mark {
      width: 40px;
      height: 40px;
      display: grid;
      place-items: center;
      background: linear-gradient(135deg, var(--gold), #ffdf8d);
      border-radius: 12px;
      color: var(--navy);
      font-size: 1.05rem;
      font-weight: 900;
      box-shadow: 0 10px 24px rgba(244, 185, 66, 0.4);
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 8px;
      flex-wrap: wrap;
    }

    .nav-links a {
      position: relative;
      padding: 10px 14px;
      color: rgba(255,255,255,0.82);
      font-size: 0.96rem;
      font-weight: 600;
      transition: color var(--transition), background var(--transition), transform var(--transition);
      border-radius: 10px;
    }

    .nav-links a:hover,
    .nav-links a:focus-visible,
    .nav-links a.active {
      color: var(--white);
      background: rgba(255,255,255,0.08);
      outline: none;
    }

    .nav-toggle {
      display: none;
      width: 48px;
      height: 48px;
      border: 1px solid rgba(255,255,255,0.2);
      border-radius: 12px;
      background: transparent;
      color: var(--white);
      cursor: pointer;
      align-items: center;
      justify-content: center;
      padding: 0;
    }

    .hamburger {
      position: relative;
      width: 22px;
      height: 2px;
      background: var(--white);
      border-radius: 2px;
    }

    .hamburger::before,
    .hamburger::after {
      content: "";
      position: absolute;
      left: 0;
      width: 22px;
      height: 2px;
      background: var(--white);
      border-radius: 2px;
      transition: transform var(--transition), opacity var(--transition);
    }

    .hamburger::before { top: -7px; }
    .hamburger::after { top: 7px; }

    .nav-toggle[aria-expanded="true"] .hamburger {
      background: transparent;
    }

    .nav-toggle[aria-expanded="true"] .hamburger::before {
      transform: translateY(7px) rotate(45deg);
    }

    .nav-toggle[aria-expanded="true"] .hamburger::after {
      transform: translateY(-7px) rotate(-45deg);
    }

    /* Hero */
    .hero {
      position: relative;
      background: linear-gradient(135deg, #0b1f3a 0%, #163763 36%, #1c4c9d 76%, #2563eb 100%);
      color: var(--white);
      overflow: hidden;
    }

    .hero::before {
      content: "";
      position: absolute;
      inset: 0;
      background:
        radial-gradient(circle at top right, rgba(244,185,66,0.2), transparent 22%),
        radial-gradient(circle at bottom left, rgba(255,255,255,0.08), transparent 24%);
      pointer-events: none;
    }

    .hero-inner {
      position: relative;
      z-index: 1;
      display: grid;
      grid-template-columns: 1.3fr 0.9fr;
      align-items: center;
      gap: 52px;
      min-height: 700px;
      padding: 64px 0;
    }

    .hero-copy {
      max-width: 640px;
    }

    .hero-badge {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: rgba(255,255,255,0.08);
      border: 1px solid rgba(255,255,255,0.15);
      padding: 8px 16px;
      border-radius: 999px;
      color: rgba(255,255,255,0.9);
      font-weight: 700;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      font-size: 0.76rem;
    }

    .hero h1 {
      margin: 18px 0 16px;
      font-size: clamp(2.7rem, 4vw, 5rem);
      line-height: 1.08;
      letter-spacing: -0.04em;
    }

    .title-highlight {
      display: inline-block;
      color: var(--gold);
    }

    .hero-intro {
      margin: 0 0 28px;
      color: rgba(255,255,255,0.82);
      font-size: 1.12rem;
      max-width: 590px;
    }

    .hero-actions {
      display: flex;
      gap: 18px;
      align-items: center;
      flex-wrap: wrap;
      margin-bottom: 30px;
    }

    .button {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      min-height: 52px;
      padding: 0 26px;
      border-radius: 999px;
      font-weight: 700;
      transition: transform var(--transition), box-shadow var(--transition), background var(--transition);
      border: 1px solid transparent;
      cursor: pointer;
    }

    .button:hover,
    .button:focus-visible {
      transform: translateY(-2px);
      outline: none;
    }

    .button-primary {
      background: linear-gradient(135deg, var(--gold), #ffd36b);
      color: var(--navy);
      box-shadow: 0 15px 32px rgba(244,185,66,0.38);
    }

    .button-secondary {
      background: rgba(255,255,255,0.06);
      color: var(--white);
      border-color: rgba(255,255,255,0.25);
    }

    .hero-meta {
      display: flex;
      gap: 18px;
      flex-wrap: wrap;
      color: rgba(255,255,255,0.8);
      font-size: 0.96rem;
    }

    .hero-meta span {
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .hero-meta .dot {
      width: 8px;
      height: 8px;
      border-radius: 50%;
      background: var(--gold);
      display: inline-block;
      box-shadow: 0 0 0 5px rgba(244,185,66,0.18);
    }

    .hero-visual {
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .portrait-card {
      position: relative;
      width: min(420px, 92%);
      padding: 18px;
      border-radius: 30px;
      background: rgba(255,255,255,0.08);
      border: 1px solid rgba(255,255,255,0.12);
      box-shadow: 0 28px 60px rgba(9, 17, 32, 0.4);
    }

    .portrait-card::before {
      content: "";
      position: absolute;
      inset: -18px auto auto -18px;
      width: 120px;
      height: 120px;
      border-radius: 28px;
      background: rgba(244,185,66,0.2);
      filter: blur(18px);
      z-index: 0;
    }

    .portrait-frame {
      position: relative;
      z-index: 1;
      overflow: hidden;
      border-radius: 24px;
      background: linear-gradient(180deg, rgba(255,255,255,0.1), rgba(255,255,255,0.02));
      border: 1px solid rgba(255,255,255,0.18);
    }

    .portrait-frame img {
      width: 100%;
      height: 560px;
      object-fit: cover;
      object-position: center top;
      filter: saturate(1.02) contrast(1.02);
    }

    .portrait-badge {
      position: absolute;
      right: 24px;
      bottom: 24px;
      background: rgba(11,31,58,0.8);
      border: 1px solid rgba(255,255,255,0.12);
      color: var(--white);
      border-radius: 18px;
      padding: 16px 18px;
      backdrop-filter: blur(8px);
      box-shadow: 0 18px 30px rgba(0,0,0,0.12);
    }

    .portrait-badge strong {
      display: block;
      font-size: 1.3rem;
      line-height: 1.2;
      color: var(--gold);
    }

    .portrait-badge span {
      color: rgba(255,255,255,0.78);
      font-size: 0.82rem;
      letter-spacing: 0.04em;
      text-transform: uppercase;
    }

    /* About */
    .about-grid {
      display: grid;
      grid-template-columns: 1.1fr 0.9fr;
      gap: 42px;
      align-items: center;
    }

    .about-copy p {
      margin: 0 0 18px;
      color: var(--muted);
      font-size: 1.06rem;
    }

    .about-points {
      margin-top: 22px;
      display: grid;
      gap: 14px;
    }

    .about-point {
      display: flex;
      align-items: flex-start;
      gap: 12px;
      padding: 18px 20px;
      background: var(--gray);
      border: 1px solid rgba(11,31,58,0.06);
      border-radius: var(--radius-md);
      box-shadow: 0 12px 24px rgba(11,31,58,0.03);
    }

    .check {
      width: 28px;
      height: 28px;
      border-radius: 50%;
      display: grid;
      place-items: center;
      background: rgba(37, 99, 235, 0.12);
      color: var(--royal);
      flex-shrink: 0;
      font-weight: 900;
      font-size: 0.9rem;
    }

    .about-card {
      background: linear-gradient(180deg, #ffffff 0%, #f4f8ff 100%);
      border: 1px solid rgba(37,99,235,0.08);
      border-radius: 26px;
      padding: 28px;
      box-shadow: var(--shadow);
    }

    .mini-label {
      display: inline-block;
      background: rgba(244,185,66,0.12);
      color: #a26d00;
      border: 1px solid rgba(244,185,66,0.2);
      border-radius: 999px;
      padding: 7px 12px;
      font-size: 0.72rem;
      font-weight: 800;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      margin-bottom: 18px;
    }

    .experience-box {
      display: grid;
      gap: 18px;
    }

    .exp-item {
      display: flex;
      gap: 14px;
      align-items: flex-start;
      padding: 16px 0;
      border-bottom: 1px solid rgba(11,31,58,0.08);
    }

    .exp-item:last-child {
      border-bottom: none;
    }

    .exp-icon {
      width: 46px;
      height: 46px;
      border-radius: 14px;
      display: grid;
      place-items: center;
      background: linear-gradient(135deg, rgba(37,99,235,0.12), rgba(11,31,58,0.04));
      color: var(--royal);
      flex-shrink: 0;
    }

    .exp-item strong {
      display: block;
      color: var(--navy);
      font-size: 1.2rem;
      margin-bottom: 2px;
    }

    .exp-item span {
      color: var(--muted);
      font-size: 0.96rem;
    }

    /* Achievements */
    .achievements {
      background: linear-gradient(180deg, #f5f8ff 0%, #edf3ff 100%);
    }

    .stats-grid {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 24px;
    }

    .stat-card {
      position: relative;
      background: var(--white);
      border: 1px solid rgba(11,31,58,0.05);
      border-radius: 22px;
      padding: 30px 24px 24px;
      box-shadow: 0 14px 30px rgba(11,31,58,0.04);
      text-align: center;
      transition: transform var(--transition), box-shadow var(--transition);
      overflow: hidden;
    }

    .stat-card:hover {
      transform: translateY(-6px);
      box-shadow: 0 18px 32px rgba(11,31,58,0.08);
    }

    .stat-card::before {
      content: "";
      position: absolute;
      inset: 0 auto auto 0;
      width: 100%;
      height: 4px;
      background: linear-gradient(90deg, var(--royal), var(--gold));
    }

    .stat-icon {
      width: 62px;
      height: 62px;
      border-radius: 18px;
      background: linear-gradient(135deg, rgba(37,99,235,0.12), rgba(244,185,66,0.12));
      display: grid;
      place-items: center;
      margin: 0 auto 20px;
      color: var(--royal);
    }

    .stat-number {
      display: block;
      font-size: clamp(2rem, 3vw, 2.8rem);
      font-weight: 800;
      line-height: 1.1;
      color: var(--navy);
      margin-bottom: 8px;
    }

    .stat-label {
      color: var(--muted);
      font-size: 1rem;
      margin: 0;
    }

    /* Expertise */
    .expertise-grid {
      display: grid;
      grid-template-columns: repeat(4, minmax(0, 1fr));
      gap: 24px;
    }

    .expertise-card {
      background: var(--white);
      border: 1px solid rgba(11,31,58,0.06);
      border-radius: 22px;
      padding: 28px 22px;
      box-shadow: 0 16px 28px rgba(11,31,58,0.04);
      transition: transform var(--transition), box-shadow var(--transition), border-color var(--transition);
    }

    .expertise-card:hover {
      transform: translateY(-6px);
      box-shadow: 0 20px 32px rgba(11,31,58,0.08);
      border-color: rgba(37,99,235,0.18);
    }

    .expertise-icon {
      width: 58px;
      height: 58px;
      display: grid;
      place-items: center;
      border-radius: 16px;
      background: linear-gradient(135deg, rgba(37,99,235,0.1), rgba(244,185,66,0.1));
      color: var(--royal);
      margin-bottom: 20px;
    }

    .expertise-card h3 {
      margin: 0 0 12px;
      font-size: 1.2rem;
      color: var(--navy);
      line-height: 1.3;
    }

    .expertise-card p {
      margin: 0;
      color: var(--muted);
      font-size: 0.97rem;
    }

    /* Core values */
    .core-values {
      background: linear-gradient(180deg, #f7f9fd 0%, #ffffff 100%);
    }

    .values-grid {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 24px;
    }

    .value-card {
      background: var(--white);
      border: 1px solid rgba(11,31,58,0.06);
      border-radius: 22px;
      padding: 28px 22px;
      box-shadow: 0 16px 28px rgba(11,31,58,0.04);
      transition: transform var(--transition), box-shadow var(--transition);
    }

    .value-card:hover {
      transform: translateY(-6px);
      box-shadow: 0 20px 34px rgba(11,31,58,0.08);
    }

    .value-icon {
      width: 58px;
      height: 58px;
      display: grid;
      place-items: center;
      border-radius: 16px;
      background: linear-gradient(135deg, rgba(37,99,235,0.12), rgba(244,185,66,0.12));
      color: var(--navy);
      margin-bottom: 18px;
    }

    .value-card h3 {
      font-size: 1.25rem;
      margin: 0 0 10px;
      color: var(--navy);
    }

    .value-card p {
      margin: 0;
      color: var(--muted);
      font-size: 0.97rem;
    }

    /* CTA */
    .cta {
      padding: 0 0 96px;
    }

    .cta-box {
      position: relative;
      overflow: hidden;
      display: grid;
      grid-template-columns: 1.6fr 0.8fr;
      align-items: center;
      gap: 24px;
      background: linear-gradient(135deg, var(--navy), #163763 60%, rgba(37,99,235,0.9));
      border-radius: 30px;
      padding: clamp(24px, 4vw, 48px);
      color: var(--white);
      box-shadow: 0 28px 50px rgba(11,31,58,0.18);
    }

    .cta-box::before {
      content: "";
      position: absolute;
      inset: 0;
      background:
        radial-gradient(circle at right center, rgba(244,185,66,0.18), transparent 26%),
        radial-gradient(circle at bottom left, rgba(255,255,255,0.08), transparent 30%);
      pointer-events: none;
    }

    .cta-content {
      position: relative;
      z-index: 1;
    }

    .cta h2 {
      margin: 0 0 12px;
      font-size: clamp(2rem, 3vw, 3rem);
      line-height: 1.15;
    }

    .cta p {
      margin: 0;
      color: rgba(255,255,255,0.8);
      font-size: 1.03rem;
      max-width: 640px;
    }

    .cta-actions {
      position: relative;
      z-index: 1;
      display: flex;
      justify-content: flex-end;
    }

    .cta .button {
      min-height: 56px;
      padding: 0 28px;
      font-size: 1.02rem;
    }

    /* Contact */
    .contact-grid {
      display: grid;
      grid-template-columns: 1.2fr 0.8fr;
      gap: 24px;
    }

    .contact-card,
    .contact-details {
      background: var(--white);
      border: 1px solid rgba(11,31,58,0.06);
      border-radius: 26px;
      box-shadow: 0 16px 28px rgba(11,31,58,0.04);
    }

    .contact-card {
      padding: 30px;
    }

    .contact-card h3,
    .contact-details h3 {
      margin: 0 0 18px;
      color: var(--navy);
      font-size: 1.5rem;
    }

    .contact-card p {
      margin: 0 0 24px;
      color: var(--muted);
      font-size: 1.02rem;
    }

    .detail-list {
      display: grid;
      gap: 18px;
    }

    .detail-item {
      display: flex;
      gap: 14px;
      align-items: flex-start;
      padding: 16px 18px;
      background: var(--gray);
      border: 1px solid rgba(11,31,58,0.04);
      border-radius: 16px;
    }

    .detail-item .icon-wrap {
      width: 42px;
      height: 42px;
      border-radius: 12px;
      background: rgba(37,99,235,0.08);
      color: var(--royal);
      display: grid;
      place-items: center;
      flex-shrink: 0;
    }

    .detail-item strong {
      display: block;
      color: var(--navy);
      margin-bottom: 4px;
      font-size: 0.96rem;
      letter-spacing: 0.02em;
    }

    .detail-item a,
    .detail-item span {
      color: var(--muted);
      font-size: 0.98rem;
    }

    .contact-details {
      padding: 30px;
      background: linear-gradient(180deg, #f7faff 0%, #ffffff 100%);
    }

    .social-btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      min-height: 52px;
      padding: 0 20px;
      border-radius: 14px;
      background: linear-gradient(135deg, #1877f2, #2563eb);
      color: var(--white);
      font-weight: 700;
      box-shadow: 0 12px 24px rgba(37,99,235,0.2);
      transition: transform var(--transition), box-shadow var(--transition);
    }

    .social-btn:hover,
    .social-btn:focus-visible {
      transform: translateY(-2px);
      box-shadow: 0 18px 28px rgba(37,99,235,0.24);
      outline: none;
    }

    /* Footer */
    .site-footer {
      background: var(--navy);
      color: rgba(255,255,255,0.78);
      padding: 28px 0 30px;
    }

    .footer-inner {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
      flex-wrap: wrap;
    }

    .footer-brand {
      display: flex;
      flex-direction: column;
      gap: 4px;
    }

    .footer-brand strong {
      color: var(--white);
      font-size: 1.1rem;
    }

    .footer-links {
      display: flex;
      align-items: center;
      gap: 18px;
      flex-wrap: wrap;
    }

    .footer-links a {
      color: rgba(255,255,255,0.8);
      transition: color var(--transition);
    }

    .footer-links a:hover,
    .footer-links a:focus-visible {
      color: var(--white);
      outline: none;
    }

    /* Reveal / animations */
    .reveal {
      opacity: 0;
      transform: translateY(24px);
      transition: opacity 0.7s ease, transform 0.7s ease;
    }

    .reveal.visible {
      opacity: 1;
      transform: translateY(0);
    }

    .delayed-1 { transition-delay: 0.05s; }
    .delayed-2 { transition-delay: 0.12s; }
    .delayed-3 { transition-delay: 0.18s; }

    @media (prefers-reduced-motion: reduce) {
      html { scroll-behavior: auto; }

      *, *::before, *::after {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
        scroll-behavior: auto !important;
      }

      .reveal {
        opacity: 1;
        transform: none;
      }
    }

    @media (max-width: 980px) {
      .hero-inner,
      .about-grid,
      .contact-grid,
      .cta-box {
        grid-template-columns: 1fr;
      }

      .expertise-grid {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }

      .values-grid {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }

      .cta-actions {
        justify-content: flex-start;
      }
    }

    @media (max-width: 760px) {
      .nav-toggle {
        display: inline-flex;
      }

      .nav-links {
        position: absolute;
        left: 12px;
        right: 12px;
        top: calc(100% + 8px);
        flex-direction: column;
        align-items: stretch;
        background: rgba(11,31,58,0.97);
        border: 1px solid rgba(255,255,255,0.08);
        border-radius: 18px;
        padding: 12px;
        box-shadow: 0 16px 34px rgba(0,0,0,0.25);
        opacity: 0;
        visibility: hidden;
        transform: translateY(-8px);
        transition: opacity var(--transition), transform var(--transition), visibility var(--transition);
      }

      .nav-links.open {
        opacity: 1;
        visibility: visible;
        transform: translateY(0);
      }

      .nav-links a {
        width: 100%;
        padding: 12px 14px;
      }

      .hero-inner {
        min-height: auto;
        padding: 52px 0 60px;
      }

      .portrait-frame img {
        height: 440px;
      }

      .stats-grid {
        grid-template-columns: 1fr;
      }

      .expertise-grid,
      .values-grid {
        grid-template-columns: 1fr;
      }

      .section {
        padding: 78px 0;
      }

      .hero-actions {
        flex-direction: column;
        align-items: stretch;
      }

      .button {
        width: 100%;
      }
    }

    @media (max-width: 520px) {
      .hero h1 {
        font-size: 2.5rem;
      }

      .hero-intro {
        font-size: 1rem;
      }

      .brand {
        font-size: 0.98rem;
      }

      .footer-inner {
        flex-direction: column;
        align-items: flex-start;
      }
    }
  </style>
</head>
<body>
  <header class="site-header">
    <div class="nav-wrap">
      <a href="#home" class="brand" aria-label="Go to home">
        <span class="brand-mark">GR</span>
        <span>Gyanwali Ramesh</span>
      </a>

      <nav aria-label="Main navigation">
        <button class="nav-toggle" aria-label="Open navigation menu" aria-expanded="false">
          <span class="hamburger"></span>
        </button>
        <div class="nav-links" id="navMenu">
          <a href="#home" class="active">Home</a>
          <a href="#about">About</a>
          <a href="#expertise">Expertise</a>
          <a href="#achievements">Achievements</a>
          <a href="#values">Core Values</a>
          <a href="#contact">Contact</a>
        </div>
      </nav>
    </div>
  </header>

  <main>
    <section id="home" class="hero">
      <div class="container hero-inner">
        <div class="hero-copy reveal">
          <div class="hero-badge">Teacher • Trainer • Digital Creator</div>
          <h1>
            Gyanwali <span class="title-highlight">Ramesh</span>
          </h1>
          <p class="hero-intro">
            A dedicated educator, management professional, and trainer committed to empowering people through practical learning, leadership, financial awareness, and digital innovation.
          </p>
          <div class="hero-actions">
            <a class="button button-primary" href="#about">Explore My Profile</a>
            <a class="button button-secondary" href="#contact">Contact Me</a>
          </div>
          <div class="hero-meta" aria-label="Professional summary">
            <span><i class="dot"></i> Teacher</span>
            <span><i class="dot"></i> Trainer</span>
            <span><i class="dot"></i> Digital Creator</span>
          </div>
        </div>

        <div class="hero-visual reveal delayed-1">
          <div class="portrait-card">
            <div class="portrait-frame">
              <img src="image.jpg" alt="Portrait of Gyanwali Ramesh, teacher, trainer, and digital creator" loading="eager" />
            </div>
            <div class="portrait-badge">
              <strong>15+</strong>
              <span>Years of Experience</span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="about" class="section">
      <div class="container">
        <div class="section-header reveal">
          <div class="eyebrow">About Me</div>
          <h2>Building knowledge, confidence, and growth</h2>
        </div>

        <div class="about-grid">
          <div class="about-copy reveal delayed-1">
            <p>
              Gyanwali Ramesh has spent over 15 years in management across different companies, teaching, and administrative leadership. He has completed more than 20 training programs as a trainer and trained over 1,000 people in management, accountancy, co-operative management, digital marketing, AI-ready training, saving and investment, and motivational development.
            </p>
            <p>
              His mission is to share knowledge, empower individuals, strengthen organizations, and help people grow through education, practical training, and digital innovation.
            </p>

            <div class="about-points">
              <div class="about-point">
                <span class="check">✓</span>
                <div>
                  <strong>Education and Management</strong><br />
                  Experienced in teaching, leadership, administration, and organizational development.
                </div>
              </div>
              <div class="about-point">
                <span class="check">✓</span>
                <div>
                  <strong>Practical Empowerment</strong><br />
                  Dedicated to helping individuals and institutions improve through skill-building and strategic learning.
                </div>
              </div>
            </div>
          </div>

          <aside class="about-card reveal delayed-2" aria-label="Professional summary">
            <span class="mini-label">Career Snapshot</span>
            <div class="experience-box">
              <div class="exp-item">
                <div class="exp-icon" aria-hidden="true">
                  <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><path d="M4 19V7.5A2.5 2.5 0 0 1 6.5 5H17.5A2.5 2.5 0 0 1 20 7.5V19M8 5V2.5M16 5V2.5M7 10H17M7 14H13" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
                </div>
                <div>
                  <strong>7+ Years</strong>
                  <span>in Accountancy</span>
                </div>
              </div>

              <div class="exp-item">
                <div class="exp-icon" aria-hidden="true">
                  <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><path d="M12 3.5L19 7V12C19 16.5 16.1 20.7 12 21.5C7.9 20.7 5 16.5 5 12V7L12 3.5Z" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/><path d="M9 12L11 14L15 10" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
                </div>
                <div>
                  <strong>10+ Years</strong>
                  <span>in Teaching</span>
                </div>
              </div>

              <div class="exp-item">
                <div class="exp-icon" aria-hidden="true">
                  <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><path d="M5 18.5V15.5C5 14.1 6.1 13 7.5 13H9.5C10.9 13 12 14.1 12 15.5V18.5M14.5 19V9.5C14.5 8.1 15.6 7 17 7H18.5C19.9 7 21 8.1 21 9.5V19M3 19H21M8 7V4.5H10.5V7M14.5 4.5H17.5" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
                </div>
                <div>
                  <strong>10+ Years</strong>
                  <span>in Co-operative Management</span>
                </div>
              </div>
            </div>
          </aside>
        </div>
      </div>
    </section>

    <section id="achievements" class="section achievements">
      <div class="container">
        <div class="section-header reveal">
          <div class="eyebrow">Achievements</div>
          <h2>Professional impact and measurable growth</h2>
        </div>

        <div class="stats-grid">
          <article class="stat-card reveal">
            <div class="stat-icon" aria-hidden="true">
              <svg width="28" height="28" viewBox="0 0 24 24" fill="none"><path d="M5 19V6.5A2.5 2.5 0 0 1 7.5 4H16.5A2.5 2.5 0 0 1 19 6.5V19M7 8H17M7 12H13M7 16H15" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <span class="stat-number" data-target="7">0</span>
            <p class="stat-label">Years in Accountancy</p>
          </article>

          <article class="stat-card reveal delayed-1">
            <div class="stat-icon" aria-hidden="true">
              <svg width="28" height="28" viewBox="0 0 24 24" fill="none"><path d="M12 3L19 7V12C19 17 16.3 20 12 21C7.7 20 5 17 5 12V7L12 3Z" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/><path d="M9 12L11 14L15 10" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <span class="stat-number" data-target="10">0</span>
            <p class="stat-label">Years in Teaching</p>
          </article>

          <article class="stat-card reveal delayed-2">
            <div class="stat-icon" aria-hidden="true">
              <svg width="28" height="28" viewBox="0 0 24 24" fill="none"><path d="M4 18.5V8.5C4 7.1 5.1 6 6.5 6H16.5C17.9 6 19 7.1 19 8.5V18.5M7 10H17M10 14H17" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/><path d="M7.5 4V2.5M16.5 4V2.5" stroke="currentColor" stroke-width="1.8" stroke-linecap="round"/></svg>
            </div>
            <span class="stat-number" data-target="10">0</span>
            <p class="stat-label">Years in Co-operative Management</p>
          </article>

          <article class="stat-card reveal">
            <div class="stat-icon" aria-hidden="true">
              <svg width="28" height="28" viewBox="0 0 24 24" fill="none"><path d="M8 6.5C8 5.1 9.1 4 10.5 4H13.5C14.9 4 16 5.1 16 6.5V7.5L18 8.5V13.5L16 14.5V18.5C16 19.9 14.9 21 13.5 21H10.5C9.1 21 8 19.9 8 18.5V14.5L6 13.5V8.5L8 7.5V6.5Z" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/><path d="M9 11H15" stroke="currentColor" stroke-width="1.8" stroke-linecap="round"/></svg>
            </div>
            <span class="stat-number" data-target="20">0</span>
            <p class="stat-label">Training Programs Completed</p>
          </article>

          <article class="stat-card reveal delayed-1">
            <div class="stat-icon" aria-hidden="true">
              <svg width="28" height="28" viewBox="0 0 24 24" fill="none"><path d="M12 6V12L16 14M21 12C21 16.97 16.97 21 12 21C7.03 21 3 16.97 3 12C3 7.03 7.03 3 12 3C16.97 3 21 7.03 21 12Z" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <span class="stat-number" data-target="1000">0</span>
            <p class="stat-label">People Trained</p>
          </article>

          <article class="stat-card reveal delayed-2">
            <div class="stat-icon" aria-hidden="true">
              <svg width="28" height="28" viewBox="0 0 24 24" fill="none"><path d="M7 18.5V13.5C7 12.1 8.1 11 9.5 11H12V19C12 20.4 10.9 21.5 9.5 21.5H7V18.5ZM12 11H14.5C15.9 11 17 12.1 17 13.5V19H14.5C13.1 19 12 17.9 12 16.5V11ZM4 19H20M9 7.5L12 4L15 7.5" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <span class="stat-number" data-target="15">0</span>
            <p class="stat-label">Years of Leadership & Management Experience</p>
          </article>
        </div>
      </div>
    </section>

    <section id="expertise" class="section">
      <div class="container">
        <div class="section-header reveal">
          <div class="eyebrow">Expertise & Training</div>
          <h2>My expertise across learning, leadership, and growth</h2>
        </div>

        <div class="expertise-grid">
          <article class="expertise-card reveal">
            <div class="expertise-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M5 18.5V8.5A2.5 2.5 0 0 1 7.5 6H16.5A2.5 2.5 0 0 1 19 8.5V18.5M7 10H17M7 14H14" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <h3>Accountancy and Financial Management</h3>
            <p>Practical training in accounting fundamentals, money management, record keeping, and financial decision-making.</p>
          </article>

          <article class="expertise-card reveal delayed-1">
            <div class="expertise-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M4 18.5V6.5C4 5.1 5.1 4 6.5 4H17.5C18.9 4 20 5.1 20 6.5V18.5M8 8H16M8 12H16M8 16H13" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <h3>Teaching and Educational Development</h3>
            <p>Learning-focused sessions designed to strengthen understanding, communication, and learner engagement.</p>
          </article>

          <article class="expertise-card reveal delayed-2">
            <div class="expertise-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M4 19V8.5A2.5 2.5 0 0 1 6.5 6H17.5A2.5 2.5 0 0 1 20 8.5V19M7 6V3.5M17 6V3.5M9 11H15M9 15H13" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <h3>Co-operative Management</h3>
            <p>Leadership and governance training aimed at improving cooperative operations, responsibilities, and accountability.</p>
          </article>

          <article class="expertise-card reveal delayed-3">
            <div class="expertise-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M5 17.5C7.5 14.5 9.4 13 12 13C14.6 13 16.5 14.5 19 17.5M8.5 10C8.5 8.1 10.1 6.5 12 6.5C13.9 6.5 15.5 8.1 15.5 10C15.5 11.9 13.9 13.5 12 13.5C10.1 13.5 8.5 11.9 8.5 10Z" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <h3>Digital Marketing</h3>
            <p>Actionable insights for online visibility, brand communication, customer engagement, and digital presence.</p>
          </article>

          <article class="expertise-card reveal">
            <div class="expertise-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M9 18.5L4.5 14L9 9.5M15 5.5L19.5 10L15 14.5" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/><path d="M13 4.5L11 19.5" stroke="currentColor" stroke-width="1.8" stroke-linecap="round"/></svg>
            </div>
            <h3>AI-Ready Training and Digital Innovation</h3>
            <p>Modern learning experiences focused on AI literacy, digital skills, and future-ready professional development.</p>
          </article>

          <article class="expertise-card reveal delayed-1">
            <div class="expertise-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M12 3.5V20.5M5 8.5H19M5 15.5H19" stroke="currentColor" stroke-width="1.8" stroke-linecap="round"/></svg>
            </div>
            <h3>Saving and Investment Awareness</h3>
            <p>Empowering people to build financial stability through practical awareness and long-term planning.</p>
          </article>

          <article class="expertise-card reveal delayed-2">
            <div class="expertise-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M7 18.5L12 5.5L17 18.5M9 14.5H15" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <h3>Leadership and Administration</h3>
            <p>Capacity-building programs for leaders, administrators, and teams seeking effective direction and management.</p>
          </article>

          <article class="expertise-card reveal delayed-3">
            <div class="expertise-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M12 4.5C9.2 4.5 7 6.7 7 9.5C7 11.6 8.2 13.4 10 14.3V18.5H14V14.3C15.8 13.4 17 11.6 17 9.5C17 6.7 14.8 4.5 12 4.5Z" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <h3>Motivation and Personal Development</h3>
            <p>Inspirational training that helps people unlock potential, build confidence, and pursue meaningful success.</p>
          </article>
        </div>
      </div>
    </section>

    <section id="values" class="section core-values">
      <div class="container">
        <div class="section-header reveal">
          <div class="eyebrow">Core Values</div>
          <h2>Principles that guide my work and leadership</h2>
        </div>

        <div class="values-grid">
          <article class="value-card reveal">
            <div class="value-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M12 21C16.5 17.2 19 14.4 19 10.8C19 7.9 16.8 5.5 14 5.5C12.5 5.5 11.2 6.1 10.5 7.1C9.8 6.1 8.5 5.5 7 5.5C4.2 5.5 2 7.9 2 10.8C2 14.4 4.5 17.2 9 21L12 23.5L15 21" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <h3>Transparent</h3>
            <p>Communicating openly and honestly.</p>
          </article>

          <article class="value-card reveal delayed-1">
            <div class="value-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M12 3.5L19 7V12C19 16.7 16.1 20.7 12 21.5C7.9 20.7 5 16.7 5 12V7L12 3.5Z" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/><path d="M9 12L11 14L15 10" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <h3>Truth-Driven</h3>
            <p>Making decisions based on facts, integrity, and evidence.</p>
          </article>

          <article class="value-card reveal delayed-2">
            <div class="value-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M8.5 10.5A3.5 3.5 0 1 1 15.5 10.5A3.5 3.5 0 1 1 8.5 10.5Z" stroke="currentColor" stroke-width="1.8"/><path d="M4 18.5C5.2 16.5 7.5 15.3 9.8 15.3H14.2C16.5 15.3 18.8 16.5 20 18.5" stroke="currentColor" stroke-width="1.8" stroke-linecap="round"/></svg>
            </div>
            <h3>Collaborative</h3>
            <p>Working together to achieve meaningful results.</p>
          </article>

          <article class="value-card reveal">
            <div class="value-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M12 4.5C8.7 4.5 6 7.2 6 10.5C6 15.5 12 19.5 12 19.5C12 19.5 18 15.5 18 10.5C18 7.2 15.3 4.5 12 4.5Z" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/><path d="M12 8V12L14.5 13.5" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <h3>Unpretentious</h3>
            <p>Staying humble, approachable, and authentic.</p>
          </article>

          <article class="value-card reveal delayed-1">
            <div class="value-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M12 3.5L18 6V11.5C18 16 15.5 19.6 12 20.5C8.5 19.6 6 16 6 11.5V6L12 3.5Z" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/><path d="M9 11L11 13L15 9" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <h3>Audacious</h3>
            <p>Embracing challenges and pursuing ambitious goals.</p>
          </article>

          <article class="value-card reveal delayed-2">
            <div class="value-icon" aria-hidden="true">
              <svg width="26" height="26" viewBox="0 0 24 24" fill="none"><path d="M4 18.5V9.5M12 18.5V5.5M20 18.5V12.5" stroke="currentColor" stroke-width="1.8" stroke-linecap="round"/></svg>
            </div>
            <h3>Growth Oriented</h3>
            <p>Continuously learning, improving, and developing.</p>
          </article>
        </div>
      </div>
    </section>

    <section class="cta">
      <div class="container">
        <div class="cta-box reveal">
          <div class="cta-content">
            <div class="eyebrow" style="background: rgba(255,255,255,0.08); color: white; border-color: rgba(255,255,255,0.15);">Collaboration</div>
            <h2>Partner with me for learning, training, and development.</h2>
            <p>
              I work with schools, organizations, institutions, and individuals to deliver practical training, capacity-building programs, leadership development, and growth-focused learning experiences.
            </p>
          </div>
          <div class="cta-actions">
            <a class="button button-primary" href="#contact">Let's Collaborate</a>
          </div>
        </div>
      </div>
    </section>

    <section id="contact" class="section">
      <div class="container">
        <div class="section-header reveal">
          <div class="eyebrow">Contact</div>
          <h2>Connect with me for training and collaboration</h2>
        </div>

        <div class="contact-grid">
          <div class="contact-card reveal">
            <h3>Get in touch</h3>
            <p>
              I am available for training, mentoring, leadership development, and professional growth programs across diverse educational and organizational settings.
            </p>

            <div class="detail-list">
              <div class="detail-item">
                <div class="icon-wrap" aria-hidden="true">
                  <svg width="20" height="20" viewBox="0 0 24 24" fill="none"><path d="M6.6 10.8C8.1 14 10.9 16.8 14.1 18.4L16.3 16.2C16.7 15.8 17.3 15.7 17.8 15.9C19.1 16.4 20.5 16.7 22 16.7C22.6 16.7 23 17.1 23 17.7V20.5C23 21.1 22.6 21.5 22 21.5C11.6 21.5 3 12.9 3 2.5C3 1.9 3.4 1.5 4 1.5H6.8C7.4 1.5 7.8 1.9 7.8 2.5C7.8 3.9 8.1 5.3 8.6 6.6C8.8 7.1 8.7 7.7 8.3 8.1L6.6 10.8Z" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"/></svg>
                </div>
                <div>
                  <strong>Phone</strong>
                  <a href="tel:+9779857037698">9857037698</a>
                </div>
              </div>

              <div class="detail-item">
                <div class="icon-wrap" aria-hidden="true">
                  <svg width="20" height="20" viewBox="0 0 24 24" fill="none"><path d="M3.5 7.5C3.5 6.1 4.6 5 6 5H18C19.4 5 20.5 6.1 20.5 7.5V16.5C20.5 17.9 19.4 19 18 19H6C4.6 19 3.5 17.9 3.5 16.5V7.5Z" stroke="currentColor" stroke-width="1.8"/><path d="M4.5 7L12 12.5L19.5 7" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
                </div>
                <div>
                  <strong>Email</strong>
                  <a href="mailto:gyanwalir@gmail.com">gyanwalir@gmail.com</a>
                </div>
              </div>

              <div class="detail-item">
                <div class="icon-wrap" aria-hidden="true">
                  <svg width="20" height="20" viewBox="0 0 24 24" fill="none"><path d="M12 21.5C16 18 20 14.4 20 9.5C20 6.5 17.5 4 14.5 4C12.8 4 11.2 4.8 10.5 6.1C9.8 4.8 8.2 4 6.5 4C3.5 4 1 6.5 1 9.5C1 14.4 5 18 9 21.5L12 24L15 21.5" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg>
                </div>
                <div>
                  <strong>Address</strong>
                  <span>Kanchan-2, Bijaya Nagar, Rupandehi, Nepal</span>
                </div>
              </div>
            </div>
          </div>

          <aside class="contact-details reveal delayed-1">
            <h3>Social Link</h3>
            <p style="margin: 0 0 22px; color: var(--muted);">
              Connect with me on Facebook to follow updates, learning resources, and professional content.
            </p>
            <a
              class="social-btn"
              href="https://www.facebook.com/share/1DJtmUdSGU/"
              target="_blank"
              rel="noopener noreferrer"
              aria-label="Open Gyanwali Ramesh Facebook profile in a new tab"
            >
              <svg width="22" height="22" viewBox="0 0 24 24" fill="none" aria-hidden="true"><path d="M13.5 22V13.5H16L16.5 10.5H13.5V8.5C13.5 7.7 13.9 7 15.2 7H16.6V4.4C16.3 4.3 15.4 4.2 14.5 4.2C12.3 4.2 10.8 5.5 10.8 8.2V10.5H8.2V13.5H10.8V22H13.5Z" fill="currentColor"/></svg>
              Facebook Profile
            </a>
          </aside>
        </div>
      </div>
    </section>
  </main>

  <footer class="site-footer">
    <div class="container footer-inner">
      <div class="footer-brand">
        <strong>Gyanwali Ramesh</strong>
        <span>Teacher | Trainer | Digital Creator</span>
      </div>

      <nav class="footer-links" aria-label="Footer navigation">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#expertise">Expertise</a>
        <a href="#achievements">Achievements</a>
        <a href="#values">Core Values</a>
        <a href="#contact">Contact</a>
      </nav>

      <div>© <span id="year"></span> Gyanwali Ramesh</div>
    </div>
  </footer>

  <script>
    const navToggle = document.querySelector('.nav-toggle');
    const navMenu = document.getElementById('navMenu');
    const navLinks = document.querySelectorAll('.nav-links a');

    if (navToggle && navMenu) {
      navToggle.addEventListener('click', () => {
        const isOpen = navMenu.classList.toggle('open');
        navToggle.setAttribute('aria-expanded', String(isOpen));
      });

      navLinks.forEach(link => {
        link.addEventListener('click', () => {
          navMenu.classList.remove('open');
          navToggle.setAttribute('aria-expanded', 'false');
        });
      });
    }

    const revealItems = document.querySelectorAll('.reveal');

    const revealObserver = new IntersectionObserver((entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
          revealObserver.unobserve(entry.target);
        }
      });
    }, {
      threshold: 0.15
    });

    revealItems.forEach(item => revealObserver.observe(item));

    const statCounters = document.querySelectorAll('.stat-number');
    const statObserver = new IntersectionObserver((entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          const el = entry.target;
          const target = Number(el.dataset.target || 0);
          const format = target >= 1000 ? value => value.toLocaleString() + '+' : value => value.toString() + '+';
          let current = 0;
          const duration = 1400;
          const startTime = performance.now();

          const tick = (time) => {
            const progress = Math.min((time - startTime) / duration, 1);
            const eased = 1 - Math.pow(1 - progress, 3);
            current = Math.round(target * eased);
            el.textContent = format(current);

            if (progress < 1) {
              requestAnimationFrame(tick);
            } else {
              el.textContent = format(target);
            }
          };

          requestAnimationFrame(tick);
          statObserver.unobserve(el);
        }
      });
    }, {
      threshold: 0.4
    });

    statCounters.forEach(counter => statObserver.observe(counter));

    const sections = document.querySelectorAll('main section[id], header section[id]');
    const navMap = [...navLinks];

    const sectionObserver = new IntersectionObserver((entries) => {
      const visibleEntries = entries.filter(entry => entry.isIntersecting);
      if (!visibleEntries.length) return;

      const currentId = visibleEntries[0].target.id;
      navMap.forEach(link => {
        const isActive = link.getAttribute('href') === `#${currentId}`;
        link.classList.toggle('active', isActive);
      });
    }, {
      rootMargin: '-35% 0px -45% 0px',
      threshold: 0.01
    });

    sections.forEach(section => sectionObserver.observe(section));

    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
