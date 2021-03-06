# Invoices payment with Testy and Cucumber

Pay your invoices with [Testy](https://github.com/sdl/Testy) ([`Selenium WebDriver`](http://www.seleniumhq.org/projects/webdriver/) test framework for web applications.) and [Cucumber](https://cucumber.io/)

## Requirements

This invoices are tested/ready for :

- [x] Cards issued @[Banca Transilvania](https://www.bancatransilvania.ro/) with [3D Secure](https://www.bancatransilvania.ro/plati-cu-cardul-pe-internet/) enabled

## Ready Scenarios

- [x] Pay [e-on](https://myline-eon.ro/) invoice
- [x] Pay [UPC](https://my.upc.ro/) invoice
- [x] Pay [DIGI](https://digicare.rcs-rds.ro/) invoice
- [x] Pay [Electrica](https://oficiulvirtual.electricafurnizare.ro/) invoice

## First Setup

- Copy:

    - [x] [src\test\resources\feature\invoice\all-invoices-demo.feature](./src/test/resources/feature/invoice/all-invoices-demo.feature) -> all-invoices.feature
    - [x] [src\test\resources\bank-card-demo.properties](./src/test/resources/bank-card-demo.properties) -> bank-card.properties
    
- Select Scenarios:

    make sure to leave only necessary scenarios
    
- Edit your credentials (user/pass/card details) into this 2 files

## Running the Tests:

    mvn clean test -Dtest=*Runner
    
## Things to improve (TODOs)

- [ ] log invoice amount
- [ ] automate first setup
- [ ] encrypt card details values
- [ ] extract user/pass in properties + encrypt
