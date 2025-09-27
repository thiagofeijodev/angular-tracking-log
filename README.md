# 📊 Angular Tracking Log

A lightweight Angular service designed to intercept and log HTTP requests and responses. Ideal for monitoring API interactions, debugging, and analyzing application behavior.

---

## 🚀 Features

* **HTTP Interception**: Automatically captures all outgoing HTTP requests and incoming responses.
* **Customizable Logging**: Easily configure logging levels and formats to suit your needs.
* **Error Handling**: Gracefully handles errors and logs relevant information for debugging.
* **Performance Monitoring**: Tracks the time taken for each request to complete.

---

## ⚙️ Installation

1. Clone the repository:

```bash
git clone https://github.com/thiagofeijodev/angular-tracking-log.git
cd angular-tracking-log
```

2. Install dependencies:

```bash
npm install
```

3. Import the `TrackingLogService` into your Angular module:

```typescript
import { TrackingLogService } from './tracking-log.service';

@NgModule({
  providers: [TrackingLogService],
})
export class AppModule {}
```

---

## 🛠️ Usage

Inject the `TrackingLogService` into your components or services where you want to log HTTP interactions:

```typescript
import { TrackingLogService } from './tracking-log.service';

@Component({
  selector: 'app-my-component',
  templateUrl: './my-component.component.html',
})
export class MyComponent {
  constructor(private trackingLog: TrackingLogService) {}

  makeRequest() {
    this.trackingLog.logRequest('GET', '/api/data');
    // Your HTTP request logic here
  }
}
```

---

## 🧪 Contributing

Contributions are welcome! Please fork the repository, create a new branch, and submit a pull request with your proposed changes.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
