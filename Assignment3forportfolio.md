{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {
    "collapsed": false
   },
   "source": [
    "#### Importing data into a data frame that we can work with."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 0,
   "metadata": {
    "collapsed": false
   },
   "outputs": [
   ],
   "source": [
    "import pandas as pd\n",
    "\n",
    "# This line makes pandas show you all of a DataFrame\n",
    "pd.set_option('display.max_columns', None)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "collapsed": false
   },
   "source": [
    "#### Reading in the data file that we want to work with"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "collapsed": false
   },
   "source": [
    "In this case, the data that we were working with was in the folder 's01' and was named 's01.txt'"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 0,
   "metadata": {
    "collapsed": false
   },
   "outputs": [
   ],
   "source": [
    "df = pd.read_csv('s01/s01.txt')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "collapsed": false
   },
   "source": [
    "#### Taking a look at our data using the pandas function head()"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 0,
   "metadata": {
    "collapsed": false
   },
   "outputs": [
   ],
   "source": [
    "df.head()"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "collapsed": false
   },
   "source": [
    "Initially looking at our data, we can see that this is likely not a format that we want to work with. To make it easier to read and easier to perform operations on, we can specify that we want to separate the data in the data frame into columns based on the key '\\t'."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 0,
   "metadata": {
    "collapsed": false
   },
   "outputs": [
   ],
   "source": [
    "df = pd.read_csv('s01/s01.txt', sep='\\t')\n",
    "df.head()"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (system-wide)",
   "language": "python",
   "metadata": {
    "cocalc": {
     "description": "Python 3 programming language",
     "priority": 100,
     "url": "https://www.python.org/"
    }
   },
   "name": "python3",
   "resource_dir": "/ext/jupyter/kernels/python3"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 4
}