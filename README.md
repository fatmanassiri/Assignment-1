# Assignment-1
this is the Python Classes i had made
I have mentioned each code with a comment to it on what it does
i kept the print and the class and objects seperate, but it still print all
there is no error
i uploaded the python classes code it is called assignment 1, thats where you will find the code
its not in readme, but it is in assignment 1
just in case you did not find it, ill paste it here



from enum import Enum #This line imports the Enum class from the enum module in Python. Enums are used to define a set of constants with a name and a value.

class Gender(Enum):
    Male = "Male"
    Female = "Female"
    Other = "Other"
#This code defines a Gender enum with three values: Male, Female, and Other.


    
class Make(Enum):
    NISSAN = "Nissan"
    TOYOTA = "Toyota"
    HONDA = "Honda"
    FORD = "Ford"
    BMW = "BMW"
    MERCEDES = "Mercedes"
#This code defines a Make enum with six values: NISSAN, TOYOTA, HONDA, FORD, BMW, and MERCEDES.
    
class Model(Enum):
    ALTIMA = "Altima"
    SENTRA = "Sentra"
    MAXIMA = "Maxima"
    CIVIC = "Civic"
    ACCORD = "Accord"
    CAMRY = "Camry"
    F150 = "F150"
    MUSTANG = "Mustang"
    X3 = "X3"
    X5 = "X5"
    C_CLASS = "C-Class"
    E_CLASS = "E-Class"
#This code defines a Model enum with twelve values: ALTIMA, SENTRA, MAXIMA, CIVIC, ACCORD, CAMRY, F150, MUSTANG, X3, X5, C_CLASS, and E_CLASS.
    
    
class ServiceName(Enum):
    DIAGNOSTICS = "Diagnostics"
    OIL_REPLACEMENT = "Oil Replacement"
    OIL_FILTER_PARTS = "Oil Filter Parts"
    TIRE_REPLACEMENT = "Tire Replacement"
    TIRE = "Tire"
#This code defines a ServiceName enum with five values: DIAGNOSTICS, OIL_REPLACEMENT, OIL_FILTER_PARTS, TIRE_REPLACEMENT, and TIRE.


    
class Currency(Enum):
    AED = "AED"
    USD = "USD"
    EUR = "EUR"
    GBP = "GBP"
    JPY = "JPY"
#This code defines a Currency enum with five values: AED, USD, EUR, GBP, and JPY.
    
class Customer:
    def __init__(self, firstName, middleInitial, lastName, phoneNumber, gender):
        self.firstName = firstName
        self.middleInitial = middleInitial
        self.lastName = lastName
        self.phoneNumber = phoneNumber
        self.gender = gender
        
    def getFirstName(self):
        return self.firstName
    
    def setFirstName(self, firstName):
        self.firstName = firstName
        
    def getMiddleInitial(self):
        return self.middleInitial
    
    def setMiddleInitial(self, middleInitial):
        self.middleInitial = middleInitial
        
    def getLastName(self):
        return self.lastName
    
    def setLastName(self, lastName):
        self.lastName = lastName
        
    def getPhoneNumber(self):
        return self.phoneNumber
    
    def setPhoneNumber(self, phoneNumber):
        self.phoneNumber = phoneNumber
        
    def getGender(self):
        return self.gender
    
    def setGender(self, gender):
        self.gender = gender
#This code defines a Customer class with a constructor that takes five parameters: firstName, middleInitial, lastName, phoneNumber, and gender. The class also has several getter and setter methods for each of these parameters.
  
        
        
# Define a Vehicle class
class Vehicle:
    # Initialize the Vehicle object with make, model, color, year, and vehicleID
    def __init__(self, make, model, color, year, vehicleID):
        self.make = make
        self.model = model
        self.color = color
        self.year = year
        self.vehicleID = vehicleID
    
    # Getter method for make
    def getMake(self):
        return self.make
    
    # Setter method for make
    def setMake(self, make):
        self.make = make
        
    # Getter method for model
    def getModel(self):
        return self.model
    
    # Setter method for model
    def setModel(self, model):
        self.model = model
        
    # Getter method for color
    def getColor(self):
        return self.color
    
    # Setter method for color
    def setColor(self, color):
        self.color = color
        
    # Getter method for year
    def getYear(self):
        return self.year
    
    # Setter method for year
    def setYear(self, year):
        self.year = year
        
    # Getter method for vehicleID
    def getVehicleID(self):
        return self.vehicleID
    
    # Setter method for vehicleID
    def setVehicleID(self, vehicleID):
        self.vehicleID = vehicleID

        
# Define a Service class
class Service:
    # Initialize the Service object with number, serviceName, itemAmount, currency, and price
    def __init__(self, number, serviceName, itemAmount, currency, price):
        self.__number = number
        self.__serviceName = serviceName
        self.__itemAmount = itemAmount
        self.__currency = currency
        self.__price = price
    
    # Getter method for number
    def getNumber(self):
        return self.__number
    
    # Setter method for number
    def setNumber(self, number):
        self.__number = number
    
    # Getter method for serviceName
    def getServiceName(self):
        return self.__serviceName
    
    # Setter method for serviceName
    def setServiceName(self, serviceName):
        self.__serviceName = serviceName
    
    # Getter method for itemAmount
    def getItemAmount(self):
        return self.__itemAmount
    
    # Setter method for itemAmount
    def setItemAmount(self, itemAmount):
        self.__itemAmount = itemAmount
    
    # Getter method for currency
    def getCurrency(self):
        return self.__currency
    
    # Setter method for currency
    def setCurrency(self, currency):
        self.__currency = currency
    
    # Getter method for price
    def getPrice(self):
        return self.__price
    
    # Setter method for price
    def setPrice(self, price):
        self.__price = price



# Payment class
class Payment:
    # Constructor method to initialize the Payment object
    def __init__(self, total, taxes, discount, finalAmount, paymentDate):
        self.__total = total
        self.__taxes = taxes
        self.__discount = discount
        self.__finalAmount = finalAmount
        self.__paymentDate = paymentDate
    
    # Getter method to return the total amount of the payment
    def getTotal(self):
        return self.__total
    
    # Setter method to set the total amount of the payment
    def setTotal(self, total):
        self.__total = total
    
    # Getter method to return the taxes applied to the payment
    def getTaxes(self):
        return self.__taxes
    
    # Setter method to set the taxes applied to the payment
    def setTaxes(self, taxes):
        self.__taxes = taxes
    
    # Getter method to return the discount applied to the payment
    def getDiscount(self):
        return self.__discount
    
    # Setter method to set the discount applied to the payment
    def setDiscount(self, discount):
        self.__discount = discount
    
    # Getter method to return the final amount after applying taxes and discounts
    def getFinalAmount(self):
        return self.__finalAmount
    
    # Setter method to set the final amount after applying taxes and discounts
    def setFinalAmount(self, finalAmount):
        self.__finalAmount = finalAmount
    
    # Getter method to return the date when the payment was made
    def getPaymentDate(self):
        return self.__paymentDate
    
    # Setter method to set the date when the payment was made
    def setPaymentDate(self, paymentDate):
        self.__paymentDate = paymentDate
        
        
# create a customer object
customer = Customer(firstName="James", lastName="Jones", middleInitial="W.", phoneNumber="816-897-9862", gender=Gender.Male)

# create a vehicle object
vehicle = Vehicle(make=Make.NISSAN, model=Model.ALTIMA, color="Silver", year="2014", vehicleID="AD-89034")

# create service objects
service1 = Service(number="1", serviceName=ServiceName.DIAGNOSTICS, itemAmount="1", currency=Currency.AED, price="15.0")
service2 = Service(number="2", serviceName=ServiceName.OIL_REPLACEMENT, itemAmount="1", currency=Currency.AED, price="120.0")
service3 = Service(number="3", serviceName=ServiceName.OIL_FILTER_PARTS, itemAmount="1", currency=Currency.AED, price="35.0")
service4 = Service(number="4", serviceName=ServiceName.TIRE_REPLACEMENT, itemAmount="2", currency=Currency.AED, price="100.0")
service5 = Service(number="5", serviceName=ServiceName.TIRE, itemAmount="2", currency=Currency.AED, price="160.0")

# create a payment object
payment = Payment(total="451.5", taxes="21.5", discount="11.5", finalAmount="440.0", paymentDate="March 13, 2022")

# print details of the customer object
print("Customer Details:")
print("First Name:", customer.getFirstName())
print("Last Name:", customer.getLastName())
print("Middle Initial:", customer.getMiddleInitial())
print("Phone Number:", customer.getPhoneNumber())
print("Gender:", customer.getGender())

# print details of the vehicle object
print("\nVehicle Details:")
print("Make:", vehicle.getMake())
print("Model:", vehicle.getModel())
print("Color:", vehicle.getColor())
print("Year:", vehicle.getYear())
print("Vehicle ID:", vehicle.getVehicleID())

# print details of the service objects
print("\nService Details:")
print("Service 1 Number:", service1.getNumber())
print("Service 1 Name:", service1.getServiceName())
print("Service 1 Amount:", service1.getItemAmount())
print("Service 1 Currency:", service1.getCurrency())
print("Service 1 Price:", service1.getPrice())

print("Service 2 Number:", service2.getNumber())
print("Service 2 Name:", service2.getServiceName())
print("Service 2 Amount:", service2.getItemAmount())
print("Service 2 Currency:", service2.getCurrency())
print("Service 2 Price:", service2.getPrice())

print("Service 3 Number:", service3.getNumber())
print("Service 3 Name:", service3.getServiceName())
print("Service 3 Amount:", service3.getItemAmount())
print("Service 3 Currency:", service3.getCurrency())
print("Service 3 Price:", service3.getPrice())

print("Service 4 Number:", service4.getNumber())
print("Service 4 Name:", service4.getServiceName())
print("Service 4 Amount:", service4.getItemAmount())
print("Service 4 Currency:", service4.getCurrency())
print("Service 4 Price:", service4.getPrice())

print("Service 5 Number:", service5.getNumber())
print("Service 5 Name:", service5.getServiceName())
print("Service 5 Amount:", service5.getItemAmount())
print("Service 5 Currency:", service5.getCurrency())
print("Service 5 Price:", service5.getPrice())

#print for the object payment
print("Payment details:")
print(f"Total: {payment.getTotal()}")
print(f"Taxes: {payment.getTaxes()}")
print(f"Discount: {payment.getDiscount()}")
print(f"Final Amount: {payment.getFinalAmount()} ")
print(f"Payment Date: {payment.getPaymentDate()}")


![image](https://user-images.githubusercontent.com/125356324/221809262-3e623efb-f19d-4e5d-b844-cf103c60e651.png)
