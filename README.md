# MITAOE Campus Library: Library Management System (prototype)

College assignment prototype (Assignment No. 3, UML Diagrams, Prototyping, Batch B-3).
A multipage static website: every page is its own `.html` file. Shared code is in `app.js` and `style.css`.

## Run it
Open `index.html` in a browser. No build step or server is needed. Data is kept in the browser's localStorage.

## Host free on GitHub Pages
1. Upload ALL files in this folder to the root of a new repository.
2. Settings > Pages > Source: "Deploy from a branch" > `main` / root > Save.
3. The site appears at `https://<username>.github.io/<repository>/`.

## Pages
- Public: `index.html`, `books.html`, `book.html?id=1`, `categories.html`, `about.html`, `login.html`
- Member: `dashboard.html`, `profile.html`, `my-books.html`, `reservations.html`, `history.html`, `fines.html`, `issue.html?id=1`
- Librarian: `admin.html`, `admin-books.html`, `admin-categories.html`, `admin-members.html`, `admin-issue.html`, `admin-return.html`, `admin-fines.html`, `admin-reservations.html`, `admin-suppliers.html`, `admin-purchases.html`, `admin-reports.html`, `admin-alerts.html`
- Supplier: `supplier.html`, `supplier-orders.html`, `supplier-books.html`, `supplier-payments.html`

## Demo logins (fictional demo data)
| Role | ID / email | Password |
|---|---|---|
| Member | `M1001` | `demo123` |
| Librarian | `librarian@campus.demo` | `admin123` |
| Supplier | `SUP001` | `demo123` |

`M1002` to `M1005` demonstrate blocked issues (overdue book, unpaid fine, loan limit).

## Notes
- Homepage statistics are the published figures from https://mitaoe.ac.in/library-our-collections.php (collection counts, not live stock).
- Catalogue, members, loans, fines, suppliers and payments are demo data. Not connected to SLIM 21.
- Loan period, fine rate and loan limit are editable demo settings, not official policy.
