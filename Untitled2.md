{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": 3,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Is 100 odd? False\n",
      "Is -1 odd? True\n"
     ]
    }
   ],
   "source": [
    "def is_odd(n):\n",
    "    return (n % 2) == 1\n",
    "\n",
    "print(\"Is 100 odd?\", is_odd(100))\n",
    "print(\"Is -1 odd?\", is_odd(-1))"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 4,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Can a 19-year-old run for president? False\n",
      "Can a 45-year-old run for president? True\n"
     ]
    }
   ],
   "source": [
    "def can_run_for_president(age):\n",
    "    \"\"\"Can someone of the given age run for president int US?\"\"\"\n",
    "    return age >= 35\n",
    "\n",
    "print(\"Can a 19-year-old run for president?\", can_run_for_president(19))\n",
    "print(\"Can a 45-year-old run for president?\", can_run_for_president(45))\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 5,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "True"
      ]
     },
     "execution_count": 5,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "3.0 == 3"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 6,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "False"
      ]
     },
     "execution_count": 6,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "'3' == 3"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 7,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Is 100 odd False\n",
      "Is -1 odd True\n"
     ]
    }
   ],
   "source": [
    "def is_odd(n):\n",
    "    return (n % 2) == 1\n",
    "\n",
    "print(\"Is 100 odd\", is_odd(100))\n",
    "print(\"Is -1 odd\", is_odd(-1))\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 12,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "4"
      ]
     },
     "execution_count": 12,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "have_umbrella = 4\n",
    "rain_level = 3\n",
    "have_hood = 1\n",
    "\n",
    "\n",
    "prepared_for_weather = have_umbrella or rain_level < 5 and have_hood or not rain_level > 0 and is_workday\n",
    "prepared_for_weather"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.6.9"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}
