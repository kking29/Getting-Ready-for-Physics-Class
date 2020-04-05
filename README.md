# Getting-Ready-for-Physics-Class
Code Academy project: You are a physics teacher preparing for the upcoming semester. You want to provide your students with some functions that will help them calculate some fundamental physical properties.


train_mass = 22680
train_acceleration = 10
train_distance = 100

bomb_mass = 1

#Turn up the Temperature
def f_to_c(f_temp):
  return (f_temp - 32) * 5/9

f100_in_celsius = f_to_c(100)

def c_to_f(c_temp):
  return (c_temp * 9/5) + 32

c0_in_fahrenheit = c_to_f(0)

#Use the Force
def get_force(mass, acceleration):
  return mass*acceleration

#Test get_force
train_force = get_force(train_mass, train_acceleration)
#Print results of train_force
print("The GE train supplies " + str(train_force) + " Newtons of force.")

#Define the fuction called get_energy
def get_energy(mass, c = 3*10**8):
  return mass*c**2

bomb_energy = get_energy(bomb_mass)
print("A 1k bomb supplies " + str(bomb_energy) + " Joules.")

#Do the work
def get_work(mass, acceleration, distance):
  force = get_force(mass,acceleration)
  return force * distance

train_work = get_work(train_mass, train_acceleration, train_distance)

#Test code
print("The GE train does " + str(train_work) + " Joules of work over " + str(train_distance) +  " meters.")


print("The GE train does " + str(train_work) + " Joules of work over " + str(train_distance) + " meters.")
