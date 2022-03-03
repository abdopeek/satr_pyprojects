import datetime
from datetime import datetime

def project():
	details = {}
	want = True
	today = datetime.today()
	final = {}
	days = {}
	count = 0

	while want is True:
		dowant = input('Do you want to add a new person (Y/N): ')
		if dowant.upper() == 'N':
			want = False
		elif dowant.upper() == 'Y':
			name = str(input('Enter the name: '))
			dateofbirth = str(input('Enter birthdate (DD-MM-YYYY): '))
			details[name] = dateofbirth
		else:
			print('enter a valid option')

	for i in range(len(list(details.keys()))):
		birth = datetime.strptime(list(details.values())[i], '%d-%m-%Y')
		age = today.year - birth.year
		day = birth.strftime('%A')
		final[list(details.keys())[i]] = age
		days[list(details.keys())[i]] = day

	names = list(final.keys())
	ages = list(final.values())
	dayss = list(days.values())

	for i in range(len(names)):
		count += 1
		print(names[i].title(),'is', ages[i],'years old and he or she is born on', dayss[i])
	if count == 1:
	    print('There is no youngest or oldest person')
	else:
	    youngest = min(ages)
	    eldest = max(ages)
	    print("The eldest is: ", names[ages.index(oldest)].title())
	    print("The youngest is: ", names[ages.index(youngest)].title())
	    print("The total amount of people is:", count)
project()
