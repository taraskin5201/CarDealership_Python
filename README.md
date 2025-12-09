# Car Dealership: Vehicle Sales Management

This application is designed for managing car sales in a dealership, including employee management, vehicle tracking, sales, and report generation. The project is developed following SOLID principles, using design patterns, and covered with PyTest-based tests.

## Main Functionality

* **Employee Management:**

  * Add a new employee
  * Edit employee information
  * Delete an employee

* **Car Management:**

  * Add a new car
  * Edit car information
  * Delete a car

* **Sales:**

  * Register a new sale
  * View all sales
  * Generate sales reports

* **Reports:**

  * Generate reports for a specific period
  * Export reports to a file

## Classes and SOLID Principles

The program is developed following SOLID principles:

1. **S - Single Responsibility Principle (SRP):**

   * `Employee`: manages employee data.
   * `Car`: stores car information.
   * `Sale`: manages sales.

2. **O - Open/Closed Principle (OCP):**

   * Classes are easily extendable via inheritance without modifying existing code.

3. **L - Liskov Substitution Principle (LSP):**

   * All subclasses (`ElectricCar`, `SportCar`) can replace the base `Car` class.

4. **I - Interface Segregation Principle (ISP):**

   * Interfaces are used for reporting, e.g., `IReportGenerator`.

5. **D - Dependency Inversion Principle (DIP):**

   * Uses abstractions (`IReportGenerator`) for report generation instead of concrete classes.

### Key Classes

* `Car`: base class for storing car information.
* `ElectricCar`: subclass of `Car` with additional parameters for electric vehicles.
* `SportCar`: subclass of `Car` for sports cars.
* `Employee`: stores dealership employee information.
* `Sale`: stores sale information (car, buyer, sale date).
* `ReportGenerator`: handles report creation.
* `CarDealership`: main class for managing the dealership.

## Usage

### Requirements

* Python 3.12
* PyTest

### Testing

The project is covered with tests using PyTest:

```bash
pytest
```

## License

MIT License
