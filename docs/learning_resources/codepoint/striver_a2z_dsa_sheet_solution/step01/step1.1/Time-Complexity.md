<style>
    #credit {
        text-align: right;
    }

    #page {
        padding: 20px;
        text-align: center;
        width: 100%;
        box-sizing: border-box;
        min-width: 1000px;
    }

    #chartTitle {
        display: inline-block;
        width: 800px;
        text-align: center;
        margin-left: 50px;
    }

    #data-structures {
        display: inline-block;
        width: 800px;
        text-align: center;
        margin-left: 50px;
    }

    #algo {
        display: inline-block;
        width: 800px;
        text-align: center;
        margin-left: 50px;
    }

    #legend {
        margin-left: 40px;
    }

    table {
        display: inline-block;
    }

    table {
        /* display: table; */
        border-collapse: separate;
        box-sizing: border-box;
        text-indent: initial;
        border-spacing: 2px;
        border-color: grey;
    }

    code {
        font-family: monospace;
    }

    table code {
        font-size: 12px;
        padding: 3px;
        font-family: Monaco, Menlo, Consolas, "Courier New", monospace;
        display: inline-block;
        border-radius: 2px;
    }

    table tr td {
        white-space: nowrap;
    }

    td {
        display: table-cell;
        vertical-align: inherit;
    }

    #legend tr td:first-child {
        text-align: center;
    }

    .md-typeset code {
        border-radius: 1rem;
    }

    .red {
        border: 1px solid #ff8989;
        color: black;
        background-color: #ff8989;
        border-width: medium;
    }

    .orange {
        border: 1px solid #FFC543;
        color: black;
        background-color: #FFC543;
        border-width: medium;
    }

    .yellow {
        border: 1px solid yellow;
        color: black;
        background-color: yellow;
        border-width: medium;
    }

    .yellow-green {
        border: 1px solid #C8EA00;
        color: black;
        background-color: #C8EA00;
        border-width: medium;
    }

    .green {
        border: 1px solid #53d000;
        color: black;
        background-color: #53d000;
        border-width: medium;
    }
</style>
<div id="page">
    <h2 id="chartTitle"> <b> Big-O Complexity Chart </b></h2>
    <div>
        <table id="legend" class="table">
            <tbody>
                <tr>
                    <td><code class="red">Horrible</code></td>
                    <td><code class="orange">Bad</code></td>
                    <td><code class="yellow">Fair</code></td>
                    <td><code class="yellow-green">Good</code></td>
                    <td><code class="green">Excellent</code></td>
                </tr>
            </tbody>
        </table>
    </div>
    <div>
        <svg id="chart" width="800" height="500" xmlns="http://www.w3.org/2000/svg">
        <!-- horrible region -->
        <path d="M50 450 L 50 0 L 800 0 L 800 450 Z" fill="#ff8989"></path>
        <!-- bad region -->
        <path d="M50 450 L 800 0 L 800 450 Z" fill="#FFC543"></path>
        <!-- fair region -->
        <path d="M50 450 L 800 450 L 800 330 Z" fill="yellow"></path>
        <!-- good region -->
        <path d="M50 450 L 800 450 L 800 410 Z" fill="#C8EA00"></path>
        <!-- excellent region -->
        <path d="M50 450 L 800 450 L 800 440 Z" fill="#53d000"></path>
        <!-- axes -->
        <path d="M50 0 L 50 450 L 800 450" fill="transparent" stroke="black" stroke-width="2"></path>
        <path d="M50 448 L 800 448" fill="transparent" stroke="black" stroke-width="2"></path>
        <text x="700" y="438" fill="black">O(log n), O(1)</text>
        <path d="M50 450 L 800 400" fill="transparent" stroke="black" stroke-width="2"></path>
        <text x="760" y="390" fill="black">O(n)</text>
        <path d="M50 450 Q 400 350, 800 150" fill="transparent" stroke="black" stroke-width="2"></path>
        <text x="630" y="190" fill="black">O(n log n)</text>
        <path d="M50 450 Q 180 380, 250 0" fill="transparent" stroke="black" stroke-width="2"></path>
        <text x="260" y="30" fill="black">O(n^2)</text>
        <path d="M50 450 C 100 430, 120 350, 120 0" fill="transparent" stroke="black" stroke-width="2"></path>
        <text x="125" y="20" fill="black">O(2^n)</text>
        <path d="M50 450 C 80 450, 80 350, 80 0" fill="transparent" stroke="black" stroke-width="2"></path>
        <text x="80" y="20" fill="black">O(n!)</text>
        <text x="0" y="0" transform="translate(30 230) rotate(-90)" style="dominant-baseline: middle; text-anchor: middle; font-size:20px; color: #555; font-size:20px; color: #555; font-style: italic;" fill="black">Operations</text>
        <text x="0" y="0" transform="translate(420 470)" style="dominant-baseline: middle; text-anchor: middle; font-size:20px; color: #555; font-style: italic;" fill="black">Elements</text>
        </svg>
    </div>
    <div id="tablesWrapper">
        <h2 id="algo"><b> Common Time Complexities </b></h2>
        <table class="table table-bordered table-striped" border="2">
            <tbody>
                <tr>
                    <th><b> Name </b></th>
                    <th><b> Time Complexity </b></th>
                </tr>
                <tr>
                    <td>Constant Time</td>
                    <td><code class="green">O(1)</code></td>
                </tr>
                <tr>
                    <td>Logarithmic Time</td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                </tr>
                <tr>
                    <td>Linear Time</td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td>Quasilinear Time</td>
                    <td><code class="orange">O(nlog(n))</code></td>
                </tr>
                <tr>
                    <td>Quadratic Time</td>
                    <td><code class="red">O(n^2)</code></td>
                </tr>
                <tr>
                    <td>Exponential Time</td>
                    <td><code class="red">O(2^n)</code></td>
                </tr>
                <tr>
                    <td>Factorial Time</td>
                    <td><code class="red">O(n!)</code></td>
                </tr>
            </tbody>
        </table>
        <h2 id="data-structures"><b> Common Data Structure Operations </b></h2>
        <table class="table table-bordered table-striped" border="2">
            <tbody>
                <tr>
                    <th>Data Structure</th>
                    <th colspan="8">Time Complexity</th>
                    <th>Space Complexity</th>
                </tr>
                <tr>
                    <th></th>
                    <th colspan="4">Average</th>
                    <th colspan="4">Worst</th>
                    <th>Worst</th>
                </tr>
                <tr>
                    <th></th>
                    <th>Access</th>
                    <th>Search</th>
                    <th>Insertion</th>
                    <th>Deletion</th>
                    <th>Access</th>
                    <th>Search</th>
                    <th>Insertion</th>
                    <th>Deletion</th>
                    <th></th>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Array_data_structure">Array</a></td>
                    <td><code class="green">Θ(1)</code></td>
                    <td><code class="yellow">Θ(n)</code></td>
                    <td><code class="yellow">Θ(n)</code></td>
                    <td><code class="yellow">Θ(n)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Singly_linked_list#Singly_linked_lists">Singly-Linked List</a></td>
                    <td><code class="yellow">Θ(n)</code></td>
                    <td><code class="yellow">Θ(n)</code></td>
                    <td><code class="green">Θ(1)</code></td>
                    <td><code class="green">Θ(1)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Doubly_linked_list">Doubly-Linked List</a></td>
                    <td><code class="yellow">Θ(n)</code></td>
                    <td><code class="yellow">Θ(n)</code></td>
                    <td><code class="green">Θ(1)</code></td>
                    <td><code class="green">Θ(1)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Skip_list">Skip List</a></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="orange">O(n log(n))</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Hash_table">Hash Table</a></td>
                    <td><code class="gray">N/A</code></td>
                    <td><code class="green">Θ(1)</code></td>
                    <td><code class="green">Θ(1)</code></td>
                    <td><code class="green">Θ(1)</code></td>
                    <td><code class="gray">N/A</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Stack_(abstract_data_type)">Stack</a></td>
                    <td><code class="yellow">Θ(n)</code></td>
                    <td><code class="yellow">Θ(n)</code></td>
                    <td><code class="green">Θ(1)</code></td>
                    <td><code class="green">Θ(1)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Queue_(abstract_data_type)">Queue</a></td>
                    <td><code class="yellow">Θ(n)</code></td>
                    <td><code class="yellow">Θ(n)</code></td>
                    <td><code class="green">Θ(1)</code></td>
                    <td><code class="green">Θ(1)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/B_tree">B-Tree</a></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Binary_search_tree">Binary Search Tree</a></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Red-black_tree">Red-Black Tree</a></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="https://en.wikipedia.org/wiki/Splay_tree">Splay Tree</a></td>
                    <td><code class="gray">N/A</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="gray">N/A</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/AVL_tree">AVL Tree</a></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="https://en.wikipedia.org/wiki/Cartesian_tree">Cartesian Tree</a></td>
                    <td><code class="gray">N/A</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="gray">N/A</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/K-d_tree">KD Tree</a></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow-green">Θ(log(n))</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
            </tbody>
        </table>
        <h2 id="algo"><b> Array Sorting Algorithms </b></h2>
        <table class="table table-bordered table-striped" border="2">
            <tbody>
                <tr>
                    <th>Algorithm</th>
                    <th colspan="3">Time Complexity</th>
                    <th>Space Complexity</th>
                </tr>
                <tr>
                    <th></th>
                    <th>Best</th>
                    <th>Average</th>
                    <th>Worst</th>
                    <th>Worst</th>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Bubble_sort">Bubble Sort</a></td>
                    <td><code class="yellow">Ω(n)</code></td>
                    <td><code class="red">Θ(n^2)</code></td>
                    <td><code class="red">O(n^2)</code></td>
                    <td><code class="green">O(1)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Insertion_sort">Insertion Sort</a></td>
                    <td><code class="yellow">Ω(n)</code></td>
                    <td><code class="red">Θ(n^2)</code></td>
                    <td><code class="red">O(n^2)</code></td>
                    <td><code class="green">O(1)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Selection_sort">Selection Sort</a></td>
                    <td><code class="red">Ω(n^2)</code></td>
                    <td><code class="red">Θ(n^2)</code></td>
                    <td><code class="red">O(n^2)</code></td>
                    <td><code class="green">O(1)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Quicksort">Quicksort</a></td>
                    <td><code class="orange">Ω(n log(n))</code></td>
                    <td><code class="orange">Θ(n log(n))</code></td>
                    <td><code class="red">O(n^2)</code></td>
                    <td><code class="yellow-green">O(log(n))</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Merge_sort">Mergesort</a></td>
                    <td><code class="orange">Ω(n log(n))</code></td>
                    <td><code class="orange">Θ(n log(n))</code></td>
                    <td><code class="orange">O(n log(n))</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Heapsort">Heapsort</a></td>
                    <td><code class="orange">Ω(n log(n))</code></td>
                    <td><code class="orange">Θ(n log(n))</code></td>
                    <td><code class="orange">O(n log(n))</code></td>
                    <td><code class="green">O(1)</code></td>
                </tr>
                <tr>
                    <td><a href="https://en.wikipedia.org/wiki/Tree_sort">Tree Sort</a></td>
                    <td><code class="orange">Ω(n log(n))</code></td>
                    <td><code class="orange">Θ(n log(n))</code></td>
                    <td><code class="red">O(n^2)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Shellsort">Shell Sort</a></td>
                    <td><code class="orange">Ω(n log(n))</code></td>
                    <td><code class="red">Θ(n(log(n))^2)</code></td>
                    <td><code class="red">O(n(log(n))^2)</code></td>
                    <td><code class="green">O(1)</code></td>
                </tr>
                <tr>
                    <td><a href="http://en.wikipedia.org/wiki/Timsort">Timsort</a></td>
                    <td><code class="yellow">Ω(n)</code></td>
                    <td><code class="orange">Θ(n log(n))</code></td>
                    <td><code class="orange">O(n log(n))</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a rel="tooltip" title="Only for integers. k is a number of buckets" href="http://en.wikipedia.org/wiki/Bucket_sort">Bucket Sort</a></td>
                    <td><code class="green">Ω(n+k)</code></td>
                    <td><code class="green">Θ(n+k)</code></td>
                    <td><code class="red">O(n^2)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
                <tr>
                    <td><a rel="tooltip" title="Constant number of digits 'k'" href="http://en.wikipedia.org/wiki/Radix_sort">Radix Sort</a></td>
                    <td><code class="green">Ω(nk)</code></td>
                    <td><code class="green">Θ(nk)</code></td>
                    <td><code class="green">O(nk)</code></td>
                    <td><code class="yellow">O(n+k)</code></td>
                </tr>
                <tr>
                    <td><a rel="tooltip" title="Difference between maximum and minimum number 'k'" href="https://en.wikipedia.org/wiki/Counting_sort">Counting Sort</a></td>
                    <td><code class="green">Ω(n+k)</code></td>
                    <td><code class="green">Θ(n+k)</code></td>
                    <td><code class="green">O(n+k)</code></td>
                    <td><code class="yellow">O(k)</code></td>
                </tr>
                <tr>
                    <td><a href="https://en.wikipedia.org/wiki/Cubesort">Cubesort</a></td>
                    <td><code class="yellow">Ω(n)</code></td>
                    <td><code class="orange">Θ(n log(n))</code></td>
                    <td><code class="orange">O(n log(n))</code></td>
                    <td><code class="yellow">O(n)</code></td>
                </tr>
            </tbody>
        </table>
        <h2 id="algo"><b> Searching Algorithms </b></h2>
        <table class="table table-bordered table-striped" border="2">
            <tbody>
                <tr>
                    <th>Algorithm</th>
                    <th colspan="2">Time Complexity</th>
                    <th>Space Complexity</th>
                </tr>
                <tr>
                    <th></th>
                    <th>Average</th>
                    <th>Worst</th>
                    <th>Worst</th>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Depth-first_search">Depth First Search (DFS)</a></td>
                    <td><code class="gray">N/A</code></td>
                    <td><code class="yellow">O(|E| + |V|)</code></td>
                    <td><code class="yellow">O(|V|)</code></td>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Breadth-first_search">Breadth First Search (BFS)</a></td>
                    <td><code class="gray">N/A</code></td>
                    <td><code class="yellow">O(|V| + |E|)</code></td>
                    <td><code class="yellow">O(|V|)</code></td>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Binary_search_algorithm">Binary Search</a></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="green">O(1)</code></td>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Linear_search">Linear Search (Brute Force)</a></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="green">O(1)</code></td>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Dijkstra's_algorithm">Shortest path Dijkstra <br> using a min-heap as priority queue</a></td>
                    <td><code class="orange">O((|V| + |E|) log|V|)</code></td>
                    <td><code class="orange">O((|V| + |E|) log|V|)</code></td>
                    <td><code class="yellow">O(|V|)</code></td>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Dijkstra's_algorithm">Shortest path Dijkstra <br> using an unsorted array as priority queue</a></td>
                    <td><code class="red">O(|V|^2)</code></td>
                    <td><code class="red">O(|V|^2)</code></td>
                    <td><code class="yellow">O(|V|)</code></td>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Bellman%E2%80%93Ford_algorithm">Shortest path by Bellman-Ford</a></td>
                    <td><code class="red">O(|V||E|)</code></td>
                    <td><code class="red">O(|V||E|)</code></td>
                    <td><code class="yellow">O(|V|)</code></td>
                </tr>
            </tbody>
        </table>
        <h2 id="algo"><b> Graphs </b></h2>
        <table class="table table-bordered table-striped" border="2">
            <tbody>
                <tr>
                    <th>Node/Edge Management</th>
                    <th colspan="6">Time Complexity</th>
                </tr>
                <tr>
                    <th></th>
                    <th>Storage</th>
                    <th>Add Vertex</th>
                    <th>Add Edge</th>
                    <th>Remove Vertex</th>
                    <th>Remove Edge</th>
                    <th>Query</th>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Adjacency_list">Adjacency List</a></td>
                    <td><code class="yellow">O(|V|+|E|)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="yellow">O(|V|+|E|)</code></td>
                    <td><code class="yellow">O(|E|)</code></td>
                    <td><code class="yellow">O(|V|)</code></td>
                </tr>
                <tr>
                    <td><a href="Incidence List">Incidence List</a></td>
                    <td><code class="yellow">O(|V|+|E|)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="yellow">O(|E|)</code></td>
                    <td><code class="yellow">O(|E|)</code></td>
                    <td><code class="yellow">O(|E|)</code></td>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Adjacency_matrix">Adjacency Matrix</a></td>
                    <td><code class="red">O(|V|^2)</code></td>
                    <td><code class="red">O(|V|^2)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="red">O(|V|^2)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="green">O(1)</code></td>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Incidence_matrix">Incidence Matrix</a></td>
                    <td><code class="red">O(|V||E|)</code></td>
                    <td><code class="red">O(|V||E|)</code></td>
                    <td><code class="red">O(|V||E|)</code></td>
                    <td><code class="red">O(|V||E|)</code></td>
                    <td><code class="red">O(|V||E|)</code></td>
                    <td><code class="yellow">O(|E|)</code></td>
                </tr>
            </tbody>
        </table>
        <h2 id="algo"><b> Heaps </b></h2>
        <table class="table table-bordered table-striped" border="2">
            <tbody>
                <tr>
                    <th>Heaps</th>
                    <th colspan="7">Time Complexity</th>
                </tr>
                <tr>
                    <th></th>
                    <th>Heapify</th>
                    <th>Find Max</th>
                    <th>Extract Max</th>
                    <th>Increase Key</th>
                    <th>Insert</th>
                    <th>Delete</th>
                    <th>Merge</th>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Linked_list">Linked List (sorted)</a></td>
                    <td><code class="gray">N/A</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="yellow">O(m+n)</code></td>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Linked_list">Linked List (unsorted)</a></td>
                    <td><code class="gray">N/A</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="green">O(1)</code></td>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Binary_heap">Binary Heap</a></td>
                    <td><code class="yellow">O(n)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="yellow">O(m+n)</code></td>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Binomial_heap">Binomial Heap</a></td>
                    <td><code class="gray">N/A</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                </tr>
                <tr>
                    <td><a href="https://www.wikiwand.com/en/Fibonacci_heap">Fibinacci Heap</a></td>
                    <td><code class="gray">N/A</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="green">O(1)</code></td>
                    <td><code class="yellow">O(log(n))</code></td>
                    <td><code class="green">O(1)</code></td>
                </tr>
            </tbody>
        </table>
    </div>
</div>
<div id="credit">
    <a href="https://www.bigocheatsheet.com/" class="md-sidebar__scrollwrap" tabindex="-1" target="_blank"> <strong>Credit : Big-O Cheat Cheat</strong> </a>
</div>