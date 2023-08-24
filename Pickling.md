# Pickling

## Introduction
Pickling is one way to perform serialization and deserialization in Python. *"Serialization is the process of converting structured data to a format that allows sharing or storage of the data in a form that allows recovery of its original structure"* [(Kenneth Reitz - External Site)](https://docs.python-guide.org/scenarios/serialization/). This can be used for machine learning so that a trained model can be serialized and reconstructed without training the model again [(Zhe Ming Chng, 2022 - External Site](https://machinelearningmastery.com/a-gentle-introduction-to-serialization-for-python/#:~:text=Serialization%20refers%20to%20the%20process,the%20reverse%20process%20of%20deserialization.)). The primary use is for maintaining data structure. Sometimes the secondary use is smaller data size, faster speed, and less energy consumption.

## Different Serialization Modules
Here is a clearly explained reason to use pickling from Davide Mastromatteo at [Real Python](https://realpython.com/python-pickle-module/) (External Site):
>"The Python pickle module is another way to serialize and deserialize objects in Python. It differs from the json module in that it serializes objects in a binary format, which means the result is not human-readable. However, it’s also faster and it works with many more Python types right out of the box, including your custom-defined objects." – Real Python

For this reason, I will create a custom object in Python and use that as an example of how pickling works.

## Custom Object Pickling
In this example, we will create a custom class in Python for a wizard’s spellbook. The pickle module will serialize and deserialize this spellbook—saving this magical knowledge for future generations.

I turned to Chat-GPT for some inspiration, then customized the script from there (Figure 1).

![Figure 1: Creating a custom class for a wizard’s spellbook.](https://github.com/DMTurnipseed/dmturnipseed.github.io/blob/gh-pages/Figure1P.png?raw=true)
Figure 1: Creating a custom class for a wizard’s spellbook.

![Figure 2: Creating spells, spellbook, and adding the spells.](https://github.com/DMTurnipseed/dmturnipseed.github.io/blob/main/Figure2P.png?raw=true)
Figure 2: Creating spells, spellbook, and adding the spells.

![Figure 3: Pickling and unpickling the spellbook.](https://github.com/DMTurnipseed/dmturnipseed.github.io/blob/main/Figure3P.png?raw=true)
Figure 3: Pickling and unpickling the spellbook.

![Figure 4: Spellbook displayed when you run the script.](https://github.com/DMTurnipseed/dmturnipseed.github.io/blob/main/Figure4P.png?raw=true)
Figure 4: Spellbook displayed when you run the script.

![Figure 5: Here is what the pickled file looks like.](https://github.com/DMTurnipseed/dmturnipseed.github.io/blob/main/Figure5P.png?raw=true)
Figure 5: Here is what the pickled file looks like.

![Figure 6: Comparing .pickle and .txt file size.](https://github.com/DMTurnipseed/dmturnipseed.github.io/blob/main/Figure6P.png?raw=true)
Figure 6: Comparing .pickle and .txt file size.

## Summary
Pickling is a module specific to Python that serializes and deserializes data into a byte stream. This is used to maintain the structure of the data and can help with file size and processing speed/power. There are other modules for serialization with their own pros and cons. One reason to choose pickling is for custom objects in Python.

## Resources
- [Zhe Ming Chng - A Gentle Introduction to Serialization in Python](https://machinelearningmastery.com/a-gentle-introduction-to-serialization-for-python/#:~:text=Serialization%20refers%20to%20the%20process,the%20reverse%20process%20of%20deserialization.)
- [Kenneth Reitz - Hitchhiker’s Guide to Python](https://docs.python-guide.org/scenarios/serialization/)
- [Python Standard Library](https://docs.python.org/3/library/pickle.html)
- [Luis, Á.; Casares, P.; Cuadrado-Gallego, J.J.; Patricio, M.A. PSON: A Serialization Format for IoT Sensor Networks. Sensors 2021, 21, 4559. https://doi.org/10.3390/s21134559](https://doi.org/10.3390/s21134559)
- [Dhaval Patel - Code Basics - Machine Learning and Pickle](https://www.youtube.com/watch?v=KfnhNlD8WZI&ab_channel=codebasics)
