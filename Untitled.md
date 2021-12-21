{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": 1,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[1, 1, 2, 3, 5, 8, 13, 21, 34, 55]\n"
     ]
    }
   ],
   "source": [
    "def fib(n):\n",
    "    \"\"\"\n",
    "    Return a list of the n Fibonacci numbers.\n",
    "    \"\"\"\n",
    "    f0, f1 = 0, 1\n",
    "    f = [1] * n\n",
    "    for i in range(1, n):\n",
    "        f[i] = f0 + f1\n",
    "        f0, f1 = f1, f[i]\n",
    "    \n",
    "    return f\n",
    "print(fib(10))"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 3,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Variable   Type        Data/Info\n",
      "--------------------------------\n",
      "fib        function    <function fib at 0x7fba4069e730>\n"
     ]
    }
   ],
   "source": [
    "%whos"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 5,
   "metadata": {},
   "outputs": [],
   "source": [
    "%lsmagic?"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 6,
   "metadata": {},
   "outputs": [
    {
     "ename": "TypeError",
     "evalue": "can't multiply sequence by non-int of type 'float'",
     "output_type": "error",
     "traceback": [
      "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
      "\u001b[0;31mTypeError\u001b[0m                                 Traceback (most recent call last)",
      "\u001b[0;32m<ipython-input-6-da4664af34ee>\u001b[0m in \u001b[0;36m<module>\u001b[0;34m()\u001b[0m\n\u001b[0;32m----> 1\u001b[0;31m \u001b[0mfib\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;36m1.0\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n\u001b[0m",
      "\u001b[0;32m<ipython-input-1-7164b007e821>\u001b[0m in \u001b[0;36mfib\u001b[0;34m(n)\u001b[0m\n\u001b[1;32m      4\u001b[0m     \"\"\"\n\u001b[1;32m      5\u001b[0m     \u001b[0mf0\u001b[0m\u001b[0;34m,\u001b[0m \u001b[0mf1\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0;36m0\u001b[0m\u001b[0;34m,\u001b[0m \u001b[0;36m1\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n\u001b[0;32m----> 6\u001b[0;31m     \u001b[0mf\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0;34m[\u001b[0m\u001b[0;36m1\u001b[0m\u001b[0;34m]\u001b[0m \u001b[0;34m*\u001b[0m \u001b[0mn\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n\u001b[0m\u001b[1;32m      7\u001b[0m     \u001b[0;32mfor\u001b[0m \u001b[0mi\u001b[0m \u001b[0;32min\u001b[0m \u001b[0mrange\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;36m1\u001b[0m\u001b[0;34m,\u001b[0m \u001b[0mn\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m:\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n\u001b[1;32m      8\u001b[0m         \u001b[0mf\u001b[0m\u001b[0;34m[\u001b[0m\u001b[0mi\u001b[0m\u001b[0;34m]\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0mf0\u001b[0m \u001b[0;34m+\u001b[0m \u001b[0mf1\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n",
      "\u001b[0;31mTypeError\u001b[0m: can't multiply sequence by non-int of type 'float'"
     ]
    }
   ],
   "source": [
    "fib(1.0)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "> \u001b[0;32m<ipython-input-1-7164b007e821>\u001b[0m(6)\u001b[0;36mfib\u001b[0;34m()\u001b[0m\n",
      "\u001b[0;32m      4 \u001b[0;31m    \"\"\"\n",
      "\u001b[0m\u001b[0;32m      5 \u001b[0;31m    \u001b[0mf0\u001b[0m\u001b[0;34m,\u001b[0m \u001b[0mf1\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0;36m0\u001b[0m\u001b[0;34m,\u001b[0m \u001b[0;36m1\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n",
      "\u001b[0m\u001b[0;32m----> 6 \u001b[0;31m    \u001b[0mf\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0;34m[\u001b[0m\u001b[0;36m1\u001b[0m\u001b[0;34m]\u001b[0m \u001b[0;34m*\u001b[0m \u001b[0mn\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n",
      "\u001b[0m\u001b[0;32m      7 \u001b[0;31m    \u001b[0;32mfor\u001b[0m \u001b[0mi\u001b[0m \u001b[0;32min\u001b[0m \u001b[0mrange\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;36m1\u001b[0m\u001b[0;34m,\u001b[0m \u001b[0mn\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m:\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n",
      "\u001b[0m\u001b[0;32m      8 \u001b[0;31m        \u001b[0mf\u001b[0m\u001b[0;34m[\u001b[0m\u001b[0mi\u001b[0m\u001b[0;34m]\u001b[0m \u001b[0;34m=\u001b[0m \u001b[0mf0\u001b[0m \u001b[0;34m+\u001b[0m \u001b[0mf1\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n",
      "\u001b[0m\n",
      "ipdb> print(n)\n",
      "1.0\n"
     ]
    }
   ],
   "source": [
    "%debug"
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
