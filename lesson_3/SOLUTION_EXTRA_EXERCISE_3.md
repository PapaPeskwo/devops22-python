# Solution

## Uppgift B

```python
from operator import itemgetter

persons = []

name_person_one = input("Please enter name for person 1:").lower()
age_person_one = int(input("Please enter age for person 1:"))
size_person_one = float(input("Please enter shoe size for person 1:"))
person_one = (name_person_one, age_person_one, size_person_one)
persons.append(person_one)

name_person_two = input("Please enter name for person 2:").lower()
age_person_two = int(input("Please enter age for person 2:"))
size_person_two = float(input("Please enter shoe size for person 2:"))
person_two = (name_person_two, age_person_two, size_person_two)
persons.append(person_two)

name_person_three = input("Please enter name for person 3:").lower()
age_person_three = int(input("Please enter age for person 3:"))
size_person_three = float(input("Please enter shoe size for person 3:"))
person_three = (name_person_three, age_person_three, size_person_three)
persons.append(person_three)

<<<<<<< HEAD:exclude/lesson_3/SOLUTION_EXTRA_EXERCISE_3.md
sorted_shoe_size = sorted(persons, key=itemgetter(1))
sorted_age = sorted(persons, key=itemgetter(2))
=======
sorted_shoe_size = sorted(persons, key=itemgetter(2))
sorted_age = sorted(persons, key=itemgetter(1))
>>>>>>> 073f9f3d51ec4b0b50d147039a039c3ad6300803:lesson_3/SOLUTION_EXTRA_EXERCISE_3.md

oldest = sorted_age[2]
median_size = sorted_shoe_size[1]

print(f"Name: {oldest[0].capitalize()}, Shoe size: {oldest[2]}")
print(f"Name: {median_size[0].capitalize()}, Age: {median_size[1]}")

<<<<<<< HEAD:exclude/lesson_3/SOLUTION_EXTRA_EXERCISE_3.md
=======
# Will only work if there are no duplicates in names, ages and sizes
>>>>>>> 073f9f3d51ec4b0b50d147039a039c3ad6300803:lesson_3/SOLUTION_EXTRA_EXERCISE_3.md
searches = {
    "age": {
        str(age_person_one): person_one,
        str(age_person_two): person_two,
        str(age_person_three): person_three
    },
<<<<<<< HEAD:exclude/lesson_3/SOLUTION_EXTRA_EXERCISE_3.md
    "shoe": {},
    "name": {}
=======
    "shoe": {
        str(size_person_one): person_one,
        str(size_person_two): person_two,
        str(size_person_three): person_three
    },
    "name": {
        str(name_person_one): person_one,
        str(name_person_two): person_two,
        str(name_person_three): person_three
    }
>>>>>>> 073f9f3d51ec4b0b50d147039a039c3ad6300803:lesson_3/SOLUTION_EXTRA_EXERCISE_3.md
}

prop, value = input("Enter prop value: ").split(" ")
print(searches[prop][value])
```
