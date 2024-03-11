                                            Text comparison idea.

The purpose of the app would be to take two writing samples and use word frequency analysis to determine if they came from the same author. A highschool teacher might use this to see if a students research paper was written by the student or AI.

Each document being complared would be a string of @ 1 page(2000 to 3000 chars) in length.

The app would interate over the string and get a count of each word ie.

    the = 65
    if = 23 
    when = 15 
    etc.. 

    The frequency of each word would be represented in a bar chart where the two documents can be visually compared.

        The would would be made with pycharts

            import pycharts
            example code

                bar_graph = pycharts.bar(title="Bar Graph Title", data=[["Value to 10", 10], ["Value to 20", 20]])
                bar_graph.savefig("bar.png")

    Streth goals

        Using a Chat GPT api to generate term papers to compare to the student paper.


    Sources 

        https://pypi.org/project/pyecharts/
        https://pycharts.readthedocs.io/en/latest/charts/bar.html