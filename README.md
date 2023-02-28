# Assignment-1
this is the Python Classes i had made
I have mentioned each code with a comment to it on what it does
i kept the print and the class and objects seperate, but it still print all
there is no error
i uploaded the python classes code it is called assignment 1, thats where you will find the code
its not in readme, but it is in assignment 1
just in case you did not find it, ill paste it here



from enum import Enum

class Gender(Enum):
    Male = "Male"
    Female = "Female"
    Other = "Other"

class Make(Enum):
    NISSAN = "Nissan"
    TOYOTA = "Toyota"
    HONDA = "Honda"
    FORD = "Ford"
    BMW = "BMW"
    MERCEDES = "Mercedes"

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
    
class ServiceName(Enum):
    DIAGNOSTICS = "Diagnostics"
    OIL_REPLACEMENT = "Oil Replacement"
    OIL_FILTER_PARTS = "Oil Filter Parts"
    TIRE_REPLACEMENT = "Tire Replacement"
    TIRE = "Tire"

class Currency(Enum):
    AED = "AED"
    USD = "USD"
    EUR = "EUR"
    GBP = "GBP"
    JPY = "JPY"
    
class Person:
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
        
    def displayInfo(self):
        print("First Name: ", self.firstName, "Middle Initial: ", self.middleInitial, " Last Name: ", self.lastName, " Phone Number: ", self.phoneNumber, " Gender: ", self.gender)
    
    

class Customer(Person):
    def __init__(self, firstName, middleInitial, lastName, phoneNumber, gender):
        super().__init__(firstName, middleInitial, lastName, phoneNumber, gender)
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

    def displayInfo(self):
        super().displayInfo()
        print("First Name: ", self.firstName, "Middle Initial: ", self.middleInitial, " Last Name: ", self.lastName, " Phone Number: ", self.phoneNumber, " Gender: ", self.gender)


class Mechanic(Person):
    def __init__(self, firstName, middleInitial, gender, serviceAmount, serviceName):
        super().__init__(firstName, middleInitial, None, None, gender)
        self.firstName = firstName
        self.middleInitial = middleInitial
        self.gender = gender
        self.serviceAmount = serviceAmount
        self.serviceName = serviceName
    
    def getFirstName(self):
        return self.firstName
    
    def setFirstName(self, firstName):
        self.firstName = firstName
        
    def getMiddleInitial(self):
        return self.middleInitial
    
    def setMiddleInitial(self, middleInitial):
        self.middleInitial = middleInitial
    
    def getGender(self):
        return self.gender
    
    def setGender(self, gender):
        self.gender = gender
        
    def getServiceAmount(self):
        return self.serviceAmount
    
    def setServiceAmount(self, serviceAmount):
        self.serviceAmount = serviceAmount
    
    def getServiceName(self):
        return self.serviceName
    
    def setServiceName(self, serviceName):
        self.serviceName = serviceName        
         
    def displayInfo(self):
        super().displayInfo()
        print("First Name: ", self.firstName, "Middle Initial: ", self.middleInitial, " Gender: ", self.gender, "Service Amount: ", self.serviceAmount, "Service Name: ", self.serviceName)
    
        
        
class Vehicle:
    def __init__(self, make, model, color, year, vehicleID):
        self.make = make
        self.model = model
        self.color = color
        self.year = year
        self.vehicleID = vehicleID
        
    def getMake(self):
        return self.make
    
    def setMake(self, make):
        self.make = make
        
    def getModel(self):
        return self.model
    
    def setModel(self, model):
        self.model = model
        
    def getColor(self):
        return self.color
    
    def setColor(self, color):
        self.color = color
        
    def getYear(self):
        return self.year
    
    def setYear(self, year):
        self.year = year
        
    def getVehicleID(self):
        return self.vehicleID
    
    def setVehicleID(self, vehicleID):
        self.vehicleID = vehicleID

    def displayInfo(self):
        print("Make: ", self.make, " Model: ", self.model, " Color: ", self.color, " Year: ", self.year, " Vehicle ID: ", self.vehicleID)


class Service:
    def __init__(self, number, serviceName, itemAmount, currency, price):
        self.__number = number
        self.__serviceName = serviceName
        self.__itemAmount = itemAmount
        self.__currency = currency
        self.__price = price
    
    def getNumber(self):
        return self.__number
    
    def setNumber(self, number):
        self.__number = number
    
    def getServiceName(self):
        return self.__serviceName
    
    def setServiceName(self, serviceName):
        self.__serviceName = serviceName
    
    def getItemAmount(self):
        return self.__itemAmount
    
    def setItemAmount(self, itemAmount):
        self.__itemAmount = itemAmount
    
    def getCurrency(self):
        return self.__currency
    
    def setCurrency(self, currency):
        self.__currency = currency
    
    def getPrice(self):
        return self.__price
    
    def setPrice(self, price):
        self.__price = price

    def displayInfo(self):
        print("Number: ", self.__number, " Service Name ", self.__serviceName, "Item Amount: ", self.__itemAmount, "Currency: ", self.__currency, "Price: ", self.__price)


class Payment:
    def __init__(self, total, taxes, discount, finalAmount, paymentDate):
        self.__total = total
        self.__taxes = taxes
        self.__discount = discount
        self.__finalAmount = finalAmount
        self.__paymentDate = paymentDate
    
    def getTotal(self):
        return self.__total
    
    def setTotal(self, total):
        self.__total = total
    
    def getTaxes(self):
        return self.__taxes
    
    def setTaxes(self, taxes):
        self.__taxes = taxes
    
    def getDiscount(self):
        return self.__discount
    
    def setDiscount(self, discount):
        self.__discount = discount
    
    def getFinalAmount(self):
        return self.__finalAmount
    
    def setFinalAmount(self, finalAmount):
        self.__finalAmount = finalAmount
    
    def getPaymentDate(self):
        return self.__paymentDate
    
    def setPaymentDate(self, paymentDate):
        self.__paymentDate = paymentDate

    def displayInfo(self):
        print("Total: ", self.__total , " Taxes: ", self.__taxes , " Discount: ", self.__discount , " Final Amount: ", self.__finalAmount , " Payment Date: ", self.__paymentDate )


person1 = Person(firstName="James", lastName="Jones", middleInitial="W", phoneNumber="123-456-7890", gender=Gender.Male)

        
customer1 = Customer(firstName="James", lastName="Jones", middleInitial="W.", phoneNumber="816-897-9862", gender=Gender.Male)

mechanic1 = Mechanic(firstName="Hans", middleInitial="K", gender= Gender.Male, serviceAmount=1, serviceName=ServiceName.DIAGNOSTICS)
mechanic2 = Mechanic(firstName="Hans", middleInitial="K", gender=Gender.Male, serviceAmount=1, serviceName=ServiceName.OIL_REPLACEMENT)
mechanic3 = Mechanic(firstName="Hans", middleInitial="K", gender=Gender.Male, serviceAmount=1, serviceName=ServiceName.OIL_FILTER_PARTS)
mechanic4 = Mechanic(firstName="Hans", middleInitial="K", gender=Gender.Male, serviceAmount=2, serviceName=ServiceName.TIRE_REPLACEMENT)
mechanic5 = Mechanic(firstName="Hans", middleInitial="K", gender=Gender.Male, serviceAmount=2, serviceName=ServiceName.TIRE)


vehicle1 = Vehicle(make=Make.NISSAN, model=Model.ALTIMA, color="Silver", year="2014", vehicleID="AD-89034")


service1 = Service(number="1", serviceName=ServiceName.DIAGNOSTICS, itemAmount="1", currency=Currency.AED, price="15.0")
service2 = Service(number="2", serviceName=ServiceName.OIL_REPLACEMENT, itemAmount="1", currency=Currency.AED, price="120.0")
service3 = Service(number="3", serviceName=ServiceName.OIL_FILTER_PARTS, itemAmount="1", currency=Currency.AED, price="35.0")
service4 = Service(number="4", serviceName=ServiceName.TIRE_REPLACEMENT, itemAmount="2", currency=Currency.AED, price="100.0")
service5 = Service(number="5", serviceName=ServiceName.TIRE, itemAmount="2", currency=Currency.AED, price="160.0")


payment1 = Payment(total="451.5", taxes="21.5", discount="11.5", finalAmount="440.0", paymentDate="March 13, 2022")


person1.displayInfo()

customer1.displayInfo()

mechanic1.displayInfo()
mechanic2.displayInfo()
mechanic3.displayInfo()
mechanic4.displayInfo()
mechanic5.displayInfo()

vehicle1.displayInfo()

service1.displayInfo()
service2.displayInfo()
service3.displayInfo()
service4.displayInfo()
service5.displayInfo()

payment1.displayInfo()
![image](https://user-images.githubusercontent.com/125356324/221908475-4727ee0f-80a3-4a79-813e-108874abc03c.png)
